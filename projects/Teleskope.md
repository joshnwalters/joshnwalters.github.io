---
layout: project
type: project
image: images/ts_logo.png
title: Teleskope
permalink: projects/Teleskope
# All dates must be YYYY-MM-DD format!
date: 2019-07-19
labels:
  - Semantic-UI
  - ReactJS
  - Meteor Web Framework
  - MongoDB
summary: Being a part of my first software engineering project
---

# Teleskope- Helping Employers find Stars
<img class="ui large rounded image" src="../images/mountain.jpg">

Teleskope is a web app that is designed to help employers find talented students from the University of Hawaii to fill their vacancies. Additionally, we envision this app being useful for students to display their skills, and see where they may be lacking in regards to skills for prospective jobs they're interested in. More information about the site can be found here.

## My Contributions

I contributed to designing and displaying the job cards that display on a companies homepage. Additionally, I implemented the modal that displays more information about the job. The cards were creating using the Semantic-UI Card element, which provides a great way to display objects to a user.

I also implemented the edit functionality for a company's profile. Using conditional rendering, a Modal button is displayed when the appropriate account is logged in. Pressing the modal button shows the modal and allows the user to modify or append information in the Companies collection.


```  submit(data) {
    const { name, owners, address, zipCode, summary, website, _id, image } = data;
    Companies.update(_id, { $set: { name, owners, address, zipCode, summary, website, image } }, (error) => (error ?
        Bert.alert({ type: 'danger', message: `Update failed: ${error.message}` }) :
        Bert.alert({ type: 'success', message: 'Update succeeded' })));
  }


  renderEditModal() {
    const { role } = this.props.profile;
    if (role !== 'company') {
      return null;
    }
    const owner = this.props.profile.owner;
    const isOwned = this.props.company.owners.includes(owner);
    if (!isOwned) {
      return null;
    }
    return <Modal id='modal' trigger={<Button
        content='Edit'
        color='green'
    />} closeIcon>
      <Grid container centered>
        <Grid.Column>
          <Header as="h2" textAlign="center">Edit Company</Header>
          <AutoForm schema={CompanySchema} onSubmit={this.submit} model={this.props.company}>
            <Segment>
              <TextField name='name'/>
              <TextField name='owners'/>
              <TextField name='address'/>
              <NumField name='zipCode' decimal={false}/>
              <TextField name='website'/>
              <TextField name='image'/>
              <LongTextField name='summary'/>
              <SubmitField value='Submit'/>
              <ErrorsField/>
            </Segment>
          </AutoForm>
        </Grid.Column>
      </Grid>
    </Modal>;
  }
  ```
## Lessons Learned
Although I had previously performed project based work before, this was my first time in a software engineering project. I had previously performed IT installation and work projects consisting of maintaining physical equipment. With software more unforeseen issues arise. I quickly learned how valuble proper planning and project management are in presenting deliverables on-time.

This was my first usage of GitHub for a team project. If we didn't have GitHub keeping track of version control, merge conflicts would have no doubt made this project take exponentially longer. 

Lastly, this was my first time developing a complex project. My previous programming projects were simple, not involving a lot of components, and usually using only one technology (Java or C). This was my first experience with both front-end and back-end programming. I guess the best lesson this taught me was I have a long way to go to be able to produce quality projects, but I'm looking forward to learning.
