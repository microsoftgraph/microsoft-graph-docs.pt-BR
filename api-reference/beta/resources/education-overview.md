---
title: Como trabalhar com APIs de educação no Microsoft Graph
description: A formação APIs no Microsoft Graph melhore os recursos do Office 365 e os dados com as informações relevantes para cenários de educação, incluindo escolas, alunos, professores, classes, inscrições e atribuições. Isso facilita a criação de soluções que se integram aos recursos educacionais.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516928"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="e4e8a-104">Como trabalhar com APIs de educação no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e4e8a-104">Working with education APIs in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e8a-105">A formação APIs no Microsoft Graph melhore os recursos do Office 365 e os dados com as informações relevantes para cenários de educação, incluindo escolas, alunos, professores, classes, inscrições e atribuições.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="e4e8a-106">Isso facilita a criação de soluções que se integram aos recursos educacionais.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="e4e8a-107">A formação APIs incluem recursos de rostering e recursos de atribuições que você pode usar para interagir com os serviços de rostering e a atribuição no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="e4e8a-108">Você pode usar estes recursos para gerenciar uma lista de participação da escola e automatizar atribuições do estudante.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-108">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="e4e8a-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-109">Authorization</span></span>

<span data-ttu-id="e4e8a-110">Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="e4e8a-111">Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="e4e8a-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="e4e8a-112">O aplicativo também precisará das permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="e4e8a-113">Para saber mais, confira [Permissões de educação](/graph/permissions-reference#education-permissions).</span><span class="sxs-lookup"><span data-stu-id="e4e8a-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="e4e8a-114">Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola</span><span class="sxs-lookup"><span data-stu-id="e4e8a-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="e4e8a-115">Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="e4e8a-116">Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="e4e8a-117">Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="e4e8a-118">Para acionar uma caixa de diálogo de consentimento, use a chamada REST a seguir.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-118">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="e4e8a-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e4e8a-119">Parameter</span></span>|<span data-ttu-id="e4e8a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="e4e8a-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="e4e8a-121">Tenant</span></span>|<span data-ttu-id="e4e8a-122">ID do locatário da escola.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-122">Tenant ID of the school.</span></span> <span data-ttu-id="e4e8a-123">Use a ID completa, que inclui onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="e4e8a-124">clientId</span><span class="sxs-lookup"><span data-stu-id="e4e8a-124">clientId</span></span>|<span data-ttu-id="e4e8a-125">ID do cliente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-125">Client ID of the app.</span></span>|
|<span data-ttu-id="e4e8a-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="e4e8a-126">redirectUrl</span></span>|<span data-ttu-id="e4e8a-127">URL de redirecionamento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="e4e8a-128">Lista de participantes</span><span class="sxs-lookup"><span data-stu-id="e4e8a-128">Rostering</span></span>

<span data-ttu-id="e4e8a-129">As APIs de lista de participantes permitem extrair dados do locatário do Office 365 de uma escola provisionado com o [Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso às informações sobre escolas, seções, professores, alunos e listas de participantes.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="e4e8a-130">As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo).</span><span class="sxs-lookup"><span data-stu-id="e4e8a-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="e4e8a-131">As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="e4e8a-132">Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="e4e8a-133">Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="e4e8a-134">Você pode usar as APIs de escalação para permitir que um usuário do aplicativo saiba:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="e4e8a-135">Quem eu sou</span><span class="sxs-lookup"><span data-stu-id="e4e8a-135">Who I am</span></span>
- <span data-ttu-id="e4e8a-136">Quais aulas eu frequento ou ministro</span><span class="sxs-lookup"><span data-stu-id="e4e8a-136">What classes I attend or teach</span></span>
- <span data-ttu-id="e4e8a-137">O que preciso fazer e quando</span><span class="sxs-lookup"><span data-stu-id="e4e8a-137">What I need to do and by when</span></span>

<span data-ttu-id="e4e8a-138">As APIs de escalação fornecem os seguintes recursos-chave:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="e4e8a-139">[educationSchool](educationschool.md) – representa a escola.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="e4e8a-140">[educationClass](educationclass.md) – representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="e4e8a-141">[educationTerm](educationterm.md) – representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="e4e8a-142">[educationTeacher](educationteacher.md) – representa um usuário com a função principal de ‘Professor’.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="e4e8a-143">[educationStudent](educationstudent.md) – representa um usuário com a função principal de 'aluno'.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="e4e8a-144">As APIs de escalação dão suporte aos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="e4e8a-145">Listar todas as escolas</span><span class="sxs-lookup"><span data-stu-id="e4e8a-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="e4e8a-146">Listar escolas nas quais uma aula é ministrada</span><span class="sxs-lookup"><span data-stu-id="e4e8a-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="e4e8a-147">Listar escolas para um usuário</span><span class="sxs-lookup"><span data-stu-id="e4e8a-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="e4e8a-148">Obter todas as aulas</span><span class="sxs-lookup"><span data-stu-id="e4e8a-148">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="e4e8a-149">Obter aulas em um escola</span><span class="sxs-lookup"><span data-stu-id="e4e8a-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="e4e8a-150">Listar aulas para um usuário</span><span class="sxs-lookup"><span data-stu-id="e4e8a-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="e4e8a-151">Adicionar aulas a uma escola</span><span class="sxs-lookup"><span data-stu-id="e4e8a-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="e4e8a-152">Obter alunos e professores para uma aula</span><span class="sxs-lookup"><span data-stu-id="e4e8a-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="e4e8a-153">Adicionar membros a uma aula</span><span class="sxs-lookup"><span data-stu-id="e4e8a-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="e4e8a-154">Listar professores para uma aula</span><span class="sxs-lookup"><span data-stu-id="e4e8a-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="e4e8a-155">Obter usuários em uma escola</span><span class="sxs-lookup"><span data-stu-id="e4e8a-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="e4e8a-156">Assignments</span><span class="sxs-lookup"><span data-stu-id="e4e8a-156">Assignments</span></span> 

<span data-ttu-id="e4e8a-157">Você pode usar a APIs de educação relacionados a atribuição de integrar com atribuições em Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="e4e8a-158">Microsoft Teams no Office 365 para educação se baseia na mesma formação APIs e fornece um caso de uso para que você pode fazer com as APIs.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-158">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="e4e8a-159">Seu aplicativo pode usar essas APIs para interagir com atribuições em todo o ciclo de vida de atribuição.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="e4e8a-160">A atribuição APIs oferecem os seguintes recursos principais:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="e4e8a-161">[educationAssignment](educationassignment.md) - o objeto de núcleo das atribuições API.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="e4e8a-162">Representa uma tarefa ou a unidade de trabalho atribuído a um estudante ou membro da equipe em uma classe como parte de sua estudo.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="e4e8a-163">[educationSubmission](educationsubmission.md) - representa os recursos que um individual (ou de grupo) envia para uma atribuição e o nível associado e comentários para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="e4e8a-164">[educationResource](educationresource.md) - representa o aprendizado do objeto ou seja sendo atribuída ou enviados.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="e4e8a-165">Um **educationResource** é associado um **educationAssignment** e/ou em um **educationSubmission**.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="e4e8a-166">A atribuição de APIs suportar os seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="e4e8a-167">Criar atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-167">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="e4e8a-168">Publicar atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="e4e8a-169">Criar o recurso de atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-169">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="e4e8a-170">Criar o recurso de envio</span><span class="sxs-lookup"><span data-stu-id="e4e8a-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="e4e8a-171">Enviar atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-171">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="e4e8a-172">Atribuição de unsubmit</span><span class="sxs-lookup"><span data-stu-id="e4e8a-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="e4e8a-173">Notas de retorno e comentários ao estudante</span><span class="sxs-lookup"><span data-stu-id="e4e8a-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="e4e8a-174">Conheça os detalhes de atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="e4e8a-175">Estes são alguns casos de uso comuns para os APIs de educação relacionados a atribuição.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-175">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="e4e8a-176">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="e4e8a-176">Use case</span></span>|<span data-ttu-id="e4e8a-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-177">Description</span></span>|<span data-ttu-id="e4e8a-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="e4e8a-178">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="e4e8a-179">Criar atribuições</span><span class="sxs-lookup"><span data-stu-id="e4e8a-179">Create assignments</span></span>|<span data-ttu-id="e4e8a-180">Um sistema externo pode criar uma atribuição para a classe e anexar recursos à atribuição.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="e4e8a-181">Criar atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-181">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="e4e8a-182">Leia as informações de atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-182">Read assignment information</span></span>|<span data-ttu-id="e4e8a-183">Um aplicativo de análise pode obter informações sobre atribuições e envios de student, incluindo datas e notas.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="e4e8a-184">Fazer a atribuição</span><span class="sxs-lookup"><span data-stu-id="e4e8a-184">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="e4e8a-185">Rastrear envios de student</span><span class="sxs-lookup"><span data-stu-id="e4e8a-185">Track student submissions</span></span>|<span data-ttu-id="e4e8a-186">Seu aplicativo pode fornecer um painel de professor que mostra quantos envios de alunos precisam ser graduadas.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="e4e8a-187">Recurso de envio</span><span class="sxs-lookup"><span data-stu-id="e4e8a-187">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="e4e8a-188">Gerenciamento de sincronização de dados de escola</span><span class="sxs-lookup"><span data-stu-id="e4e8a-188">School data sync management</span></span>

<span data-ttu-id="e4e8a-189">[Sincronização de dados da escola](https://sds.microsoft.com/) ajuda a automatizar o processo de importação e a sincronização de dados de lista de participação de sistemas de informação de student com o Azure Active Directory (AD Azure) e Office 365.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-189">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="e4e8a-190">Você pode usar o gerenciamento de sincronização de dados escola APIs no Microsoft Graph para configurar a sincronização de um arquivo CSV ou um conector de API SIS com suporte.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-190">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="e4e8a-191">Os dados da escola sincronizar o suporte ao gerenciamento de APIs os seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-191">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="e4e8a-192">Perfis de sincronização de lista</span><span class="sxs-lookup"><span data-stu-id="e4e8a-192">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="e4e8a-193">Obtenha o perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-193">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="e4e8a-194">Criar um perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-194">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="e4e8a-195">Excluir o perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-195">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="e4e8a-196">Pausar uma sincronização em andamento</span><span class="sxs-lookup"><span data-stu-id="e4e8a-196">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="e4e8a-197">Retomar uma sincronização pausada</span><span class="sxs-lookup"><span data-stu-id="e4e8a-197">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="e4e8a-198">Redefinir uma sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-198">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="e4e8a-199">Iniciar sincronização para arquivos carregados</span><span class="sxs-lookup"><span data-stu-id="e4e8a-199">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="e4e8a-200">Obtenha uma URL de carregamento</span><span class="sxs-lookup"><span data-stu-id="e4e8a-200">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="e4e8a-201">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-201">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="e4e8a-202">Obtenha os erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="e4e8a-202">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="e4e8a-203">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e4e8a-203">Next steps</span></span>
<span data-ttu-id="e4e8a-204">Use a APIs de educação do Microsoft Graph para construir soluções de educação que acessam as atribuições do estudante e escalações escola.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-204">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="e4e8a-205">Para saber mais:</span><span class="sxs-lookup"><span data-stu-id="e4e8a-205">To learn more:</span></span>

- <span data-ttu-id="e4e8a-206">Explore os recursos e os métodos mais úteis para seu cenário.</span><span class="sxs-lookup"><span data-stu-id="e4e8a-206">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="e4e8a-207">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="e4e8a-207">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
