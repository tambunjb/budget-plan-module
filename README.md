# <span id="tjidtitle">Budget Plan Module</span>

<div>Technologies: <span id="tjidtechs">Yii2, MySQL</span></div>
<br />

This is a module for managing budgets that I created in 2018. Everyone in the organization needs to plan what they're going to do next year and how much money they'll need for it. They also have to figure out where the money will come from, break down the costs, and discuss it with their boss. All of these features need to be handled in the system. So, this module is all about making it possible to create this information and for different parts of the organization to work together.

Let's start with how the data is organized in this tool. There are 7 main tables, not counting reference tables:
<p align="center">
<img width="60%" alt="mata_anggaran" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/1aad4593-c44e-4e73-a9c1-b7ad59e600f0">
</p>
1. mata_anggaran: budget item, where money will be allocated.<br />
2. struktur_jabatan_has_mata_anggaran: specific budget items assigned to different roles in the organization.<br />
3. program: the activities or plans that will be carried out.<br />
4. program_has_sumber_dana: shows where the money for the programs is coming from.<br />
5. program_has_waktu: specifies when the planned programs will take place.<br />
6. detil_program: breaks down the programs into smaller details.<br />
7. review_program: the assessments made for the programs.<br />
<br />
Now, let's look at the steps in using the module :
<br /><br />
Managing Budget Items: This is where you can create, update, delete, or view budget items.
<p align="center">
<img width="60%" alt="mata_anggaran" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/7a42f8b4-edd3-4bf9-b791-5a64b6d16624">
</p>
<br />
Assigning Budget Items to Roles: Here, you can link budget items to specific roles, allowing users in those roles to create programs using the assigned budget items.
<p align="center">
<img width="60%" alt="penugasan_anggaran" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/1954131c-8acd-49c2-90cd-0c31f245aa19">
</p>
<br />
Creating a Program: Users can create programs themselves or request someone else to create a program. The status of a program will be "draft" until it's accepted by the requested user.
<p align="center">
<img width="60%" alt="create_program" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/264ce86a-0fad-4617-9c90-6ba76ddc6ad9">
</p>
<br />
Breaking Down Programs: Programs can be divided into smaller parts for better management.
<p align="center">
<img width="60%" alt="breakdown_program" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/4e737cb5-c159-4944-b843-44630ca8a09d">
</p>
<br />
List of Programs: This shows all the programs, allowing users to accept or review drafts made by others based on the organization's structure.
<p align="center">
<img width="60%" alt="index_accept_compilation" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/6a3534a8-e276-436d-abc8-043e7c6d1f35">
</p>
<br />
Supervisory Reviews: This section allows superiors to review programs created by their subordinates.
<p align="center">
<img width="60%" alt="review_program" src="https://github.com/tambunjb/budget-plan-module/assets/22196181/c1892e38-a1e7-4361-9c7b-9b3f9eb4e546">
</p>
<br />
This tool uses the organization's structure to determine who can accept, review, or reject programs. It also helps identify the main supervisor who can view all the organization's programs in detail along with their statuses.

