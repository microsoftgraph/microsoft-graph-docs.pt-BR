---
title: Como trabalhar com APIs de educação no Microsoft Graph
description: As APIs de educação no Microsoft Graph aprimoram os recursos e dados do Microsoft 365 com informações que são relevantes para cenários de educação, incluindo escolas, alunos, professores, aulas e matrículas. Isso facilita a criação de soluções que se integram aos recursos educacionais.
localization_priority: Priority
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 1bfe49d6841142794a5b3a60b0de84eaff4290d4
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231529"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="5a1f1-104">Como trabalhar com APIs de educação no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5a1f1-104">Working with education APIs in Microsoft Graph</span></span>

<span data-ttu-id="5a1f1-105">As APIs de educação no Microsoft Graph aprimoram os recursos e dados do Microsoft 365 com informações que são relevantes para cenários de educação, incluindo escolas, alunos, professores, aulas e matrículas.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-105">The education APIs in Microsoft Graph enhance Microsoft 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="5a1f1-106">Isso facilita a criação de soluções que se integram aos recursos educacionais.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="5a1f1-p103">As APIs de educação incluem recursos de listagem e recursos de tarefas que você pode usar para interagir com os serviços de listagem no Microsoft Teams. Você pode usar esses recursos para gerenciar uma lista de escolas.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-p103">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams. You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="5a1f1-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a1f1-109">Authorization</span></span>

<span data-ttu-id="5a1f1-110">Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="5a1f1-111">Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](/graph/auth/).</span><span class="sxs-lookup"><span data-stu-id="5a1f1-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="5a1f1-112">O aplicativo também precisará das permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="5a1f1-113">Para saber mais, confira [Permissões de educação](/graph/permissions-reference#education-permissions).</span><span class="sxs-lookup"><span data-stu-id="5a1f1-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span>

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="5a1f1-114">Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola</span><span class="sxs-lookup"><span data-stu-id="5a1f1-114">App permissions to enable school IT admins to consent</span></span>

<span data-ttu-id="5a1f1-115">Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="5a1f1-116">Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="5a1f1-117">Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="5a1f1-118">Para mostrar uma caixa de diálogo de consentimento, use a chamada REST a seguir.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-118">To show a consent dialog box, use the following REST call.</span></span>

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| <span data-ttu-id="5a1f1-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a1f1-119">Parameter</span></span>   | <span data-ttu-id="5a1f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a1f1-120">Description</span></span>                                                               |
| :---------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="5a1f1-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="5a1f1-121">Tenant</span></span>      | <span data-ttu-id="5a1f1-122">ID do locatário da escola.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-122">Tenant ID of the school.</span></span> <span data-ttu-id="5a1f1-123">Use a ID completa, que inclui onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-123">Use the full ID, which includes onmicrosoft.com.</span></span> |
| <span data-ttu-id="5a1f1-124">clientId</span><span class="sxs-lookup"><span data-stu-id="5a1f1-124">clientId</span></span>    | <span data-ttu-id="5a1f1-125">ID do cliente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-125">Client ID of the app.</span></span>                                                     |
| <span data-ttu-id="5a1f1-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="5a1f1-126">redirectUrl</span></span> | <span data-ttu-id="5a1f1-127">URL de redirecionamento do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-127">App redirect URL.</span></span>                                                         |

## <a name="rostering"></a><span data-ttu-id="5a1f1-128">Lista de participantes</span><span class="sxs-lookup"><span data-stu-id="5a1f1-128">Rostering</span></span>

<span data-ttu-id="5a1f1-129">As APIs de lista de participantes permitem extrair dados do locatário do Microsoft 365 de uma escola provisionado com o [Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso às informações sobre escolas, seções, professores, alunos e listas de participantes.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-129">The rostering APIs enable you to extract data from a school's Microsoft 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="5a1f1-130">As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo).</span><span class="sxs-lookup"><span data-stu-id="5a1f1-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="5a1f1-131">As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="5a1f1-132">Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="5a1f1-133">Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="5a1f1-134">Você pode usar as APIs de escalação para permitir que um usuário do aplicativo saiba:</span><span class="sxs-lookup"><span data-stu-id="5a1f1-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="5a1f1-135">Quem eu sou</span><span class="sxs-lookup"><span data-stu-id="5a1f1-135">Who I am</span></span>
- <span data-ttu-id="5a1f1-136">Quais aulas eu frequento ou ministro</span><span class="sxs-lookup"><span data-stu-id="5a1f1-136">What classes I attend or teach</span></span>
- <span data-ttu-id="5a1f1-137">O que preciso fazer e quando</span><span class="sxs-lookup"><span data-stu-id="5a1f1-137">What I need to do and by when</span></span>

<span data-ttu-id="5a1f1-138">As APIs de escalação fornecem os seguintes recursos-chave:</span><span class="sxs-lookup"><span data-stu-id="5a1f1-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="5a1f1-139">[educationSchool](educationschool.md) – representa a escola.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="5a1f1-140">[educationClass](educationclass.md) – representa uma aula em uma escola.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="5a1f1-141">[educationTerm](educationterm.md) – representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="5a1f1-142">[educationTeacher](educationteacher.md) – representa um usuário com a função principal de ‘Professor’.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-142">[educationTeacher](educationteacher.md) - Represents a user with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="5a1f1-143">[educationStudent](educationstudent.md) – representa um usuário com a função principal de 'aluno'.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-143">[educationStudent](educationstudent.md) - Represents a user with the primary role of 'student'.</span></span>

<span data-ttu-id="5a1f1-144">As APIs de escalação dão suporte aos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="5a1f1-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="5a1f1-145">Listar todas as escolas</span><span class="sxs-lookup"><span data-stu-id="5a1f1-145">List all schools</span></span>](../api/educationschool-list.md)
- [<span data-ttu-id="5a1f1-146">Listar escolas nas quais uma aula é ministrada</span><span class="sxs-lookup"><span data-stu-id="5a1f1-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="5a1f1-147">Listar escolas para um usuário</span><span class="sxs-lookup"><span data-stu-id="5a1f1-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="5a1f1-148">Obter todas as aulas</span><span class="sxs-lookup"><span data-stu-id="5a1f1-148">Get all classes</span></span>](../api/educationclass-list.md)
- [<span data-ttu-id="5a1f1-149">Obter aulas em um escola</span><span class="sxs-lookup"><span data-stu-id="5a1f1-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="5a1f1-150">Listar aulas para um usuário</span><span class="sxs-lookup"><span data-stu-id="5a1f1-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="5a1f1-151">Adicionar aulas a uma escola</span><span class="sxs-lookup"><span data-stu-id="5a1f1-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="5a1f1-152">Obter alunos e professores para uma aula</span><span class="sxs-lookup"><span data-stu-id="5a1f1-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="5a1f1-153">Adicionar membros a uma aula</span><span class="sxs-lookup"><span data-stu-id="5a1f1-153">Add members to a class</span></span>](../api/educationclass-post-members.md)
- [<span data-ttu-id="5a1f1-154">Listar professores para uma aula</span><span class="sxs-lookup"><span data-stu-id="5a1f1-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="5a1f1-155">Obter usuários em uma escola</span><span class="sxs-lookup"><span data-stu-id="5a1f1-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="whats-new"></a><span data-ttu-id="5a1f1-156">O que há de novo</span><span class="sxs-lookup"><span data-stu-id="5a1f1-156">What's new</span></span>

<span data-ttu-id="5a1f1-157">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-157">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5a1f1-158">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5a1f1-158">Next steps</span></span>

<span data-ttu-id="5a1f1-p108">Use as APIs de educação do Microsoft Graph para construir soluções educacionais que acessam as listas escolares. Para saber mais:</span><span class="sxs-lookup"><span data-stu-id="5a1f1-p108">Use the Microsoft Graph education APIs to build education solutions that access school rosters. To learn more:</span></span>

- <span data-ttu-id="5a1f1-161">Explore os recursos e os métodos mais úteis para seu cenário.</span><span class="sxs-lookup"><span data-stu-id="5a1f1-161">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="5a1f1-162">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="5a1f1-162">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
