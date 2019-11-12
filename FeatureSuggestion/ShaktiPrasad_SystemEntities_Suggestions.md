#### This may not cover all required entities. Just putting forward my thoughts.

#### Class Section
{
````
	string title;
	string paragraph;(rich text)
	Public:
		Section(title, paragraph)
		void setTitle();
		void getTitle();
		void setParagraph();
		void getParagraph();
````
}

#### Class Resume
{
````
	/* This is a base class,Each template shall inherit this, additonal sections vars can be added to each template. */

	/*
	Each template can have 
	some fixed sections.
	*/
	Section personalInfo;
	Section education;
	Section workExperince;
	Section Projects;
	Section Skills;
	/*
	Dynamic array.
	New sections can be added or removed.
	*/
	Section AdditonalSections[]; 

	Public:
		Getters & Setters for attributes.
		AddSection();
		RemoveSection();
````
}

#### We should have an UI interface to create a resume child class and add/remove sections. 
