---
title: Criar educationClass
description: Crie um novo objeto educationClass.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71dcda18e56b6dfd53fa35943e6da246b5b8d68f
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232148"
---
# <a name="create-educationclass"></a><span data-ttu-id="6e38b-103">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="6e38b-103">Create educationClass</span></span>

<span data-ttu-id="6e38b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e38b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e38b-105">Crie um novo [objeto educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="6e38b-105">Create a new [educationClass](../resources/educationclass.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="6e38b-106">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="6e38b-106">This will also create a universal group.</span></span> <span data-ttu-id="6e38b-107">Quando você usa essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams quando as equipes são criadas usando o grupo.</span><span class="sxs-lookup"><span data-stu-id="6e38b-107">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="6e38b-108">Observe que essa API cria apenas o grupo universal e não cria uma equipe.</span><span class="sxs-lookup"><span data-stu-id="6e38b-108">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="6e38b-109">Microsoft Teams fornece uma interface de usuário para que os professores criem equipes para suas próprias classes usando os grupos criados por essa API.</span><span class="sxs-lookup"><span data-stu-id="6e38b-109">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e38b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e38b-110">Permissions</span></span>

<span data-ttu-id="6e38b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e38b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e38b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e38b-113">Permission type</span></span>                        | <span data-ttu-id="6e38b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e38b-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6e38b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e38b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e38b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e38b-116">Not supported.</span></span>                              |
| <span data-ttu-id="6e38b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e38b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e38b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e38b-118">Not supported.</span></span>                              |
| <span data-ttu-id="6e38b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e38b-119">Application</span></span>                            | <span data-ttu-id="6e38b-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e38b-120">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="6e38b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e38b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a><span data-ttu-id="6e38b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e38b-122">Request headers</span></span>

| <span data-ttu-id="6e38b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6e38b-123">Name</span></span>          | <span data-ttu-id="6e38b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e38b-124">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="6e38b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e38b-125">Authorization</span></span> | <span data-ttu-id="6e38b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e38b-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6e38b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e38b-128">Content-Type</span></span>  | <span data-ttu-id="6e38b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e38b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e38b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e38b-131">Request body</span></span>

<span data-ttu-id="6e38b-132">No corpo da solicitação, fornece uma representação JSON do [objeto educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="6e38b-132">In the request body, supply a JSON representation of the [educationClass](../resources/educationclass.md) object.</span></span>

<span data-ttu-id="6e38b-133">A tabela a seguir mostra as propriedades que são necessárias ao criar [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="6e38b-133">The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).</span></span>

| <span data-ttu-id="6e38b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e38b-134">Property</span></span>             | <span data-ttu-id="6e38b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e38b-135">Type</span></span>                                           | <span data-ttu-id="6e38b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e38b-136">Description</span></span>                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="6e38b-137">id</span><span class="sxs-lookup"><span data-stu-id="6e38b-137">id</span></span>                   | <span data-ttu-id="6e38b-138">String</span><span class="sxs-lookup"><span data-stu-id="6e38b-138">String</span></span>                                         | <span data-ttu-id="6e38b-139">Identificador de objeto.</span><span class="sxs-lookup"><span data-stu-id="6e38b-139">Object identifier.</span></span> <span data-ttu-id="6e38b-140">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="6e38b-140">Inherited from [entity](../resources/entity.md)</span></span> |
| <span data-ttu-id="6e38b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6e38b-141">displayName</span></span>          | <span data-ttu-id="6e38b-142">String</span><span class="sxs-lookup"><span data-stu-id="6e38b-142">String</span></span>                                         | <span data-ttu-id="6e38b-143">Nome da aula.</span><span class="sxs-lookup"><span data-stu-id="6e38b-143">Name of the class.</span></span>                                                 |
| <span data-ttu-id="6e38b-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6e38b-144">mailNickname</span></span>         | <span data-ttu-id="6e38b-145">String</span><span class="sxs-lookup"><span data-stu-id="6e38b-145">String</span></span>                                         | <span data-ttu-id="6e38b-146">Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="6e38b-146">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="6e38b-147">descrição</span><span class="sxs-lookup"><span data-stu-id="6e38b-147">description</span></span>          | <span data-ttu-id="6e38b-148">String</span><span class="sxs-lookup"><span data-stu-id="6e38b-148">String</span></span>                                         | <span data-ttu-id="6e38b-149">Descrição da aula.</span><span class="sxs-lookup"><span data-stu-id="6e38b-149">Description of the class.</span></span>                                          |
| <span data-ttu-id="6e38b-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="6e38b-150">createdBy</span></span>            | [<span data-ttu-id="6e38b-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="6e38b-151">identitySet</span></span>](../resources/identityset.md)     | <span data-ttu-id="6e38b-152">Entidade que criou a aula</span><span class="sxs-lookup"><span data-stu-id="6e38b-152">Entity who created the class</span></span>                                       |
| <span data-ttu-id="6e38b-153">classCode</span><span class="sxs-lookup"><span data-stu-id="6e38b-153">classCode</span></span>            | <span data-ttu-id="6e38b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e38b-154">String</span></span>                                         | <span data-ttu-id="6e38b-155">Código de aula usada pela escola para identificar a aula.</span><span class="sxs-lookup"><span data-stu-id="6e38b-155">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="6e38b-156">externalName</span><span class="sxs-lookup"><span data-stu-id="6e38b-156">externalName</span></span>         | <span data-ttu-id="6e38b-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e38b-157">String</span></span>                                         | <span data-ttu-id="6e38b-158">Nome da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6e38b-158">Name of the class in the syncing system.</span></span>                           |
| <span data-ttu-id="6e38b-159">externalId</span><span class="sxs-lookup"><span data-stu-id="6e38b-159">externalId</span></span>           | <span data-ttu-id="6e38b-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e38b-160">String</span></span>                                         | <span data-ttu-id="6e38b-161">ID da aula no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6e38b-161">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="6e38b-162">externalSource</span><span class="sxs-lookup"><span data-stu-id="6e38b-162">externalSource</span></span>       | <span data-ttu-id="6e38b-163">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6e38b-163">educationExternalSource</span></span>                        | <span data-ttu-id="6e38b-164">Como essa aula foi criada.</span><span class="sxs-lookup"><span data-stu-id="6e38b-164">How this class was created.</span></span> <span data-ttu-id="6e38b-165">Os valores possíveis são: `sis` , `manual`</span><span class="sxs-lookup"><span data-stu-id="6e38b-165">Possible values are: `sis`, `manual`</span></span>   |
| <span data-ttu-id="6e38b-166">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="6e38b-166">externalSourceDetail</span></span> | <span data-ttu-id="6e38b-167">String</span><span class="sxs-lookup"><span data-stu-id="6e38b-167">String</span></span>                                         | <span data-ttu-id="6e38b-168">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="6e38b-168">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="6e38b-169">grade</span><span class="sxs-lookup"><span data-stu-id="6e38b-169">grade</span></span>                | <span data-ttu-id="6e38b-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e38b-170">String</span></span>                                         | <span data-ttu-id="6e38b-171">Nível de nota da classe.</span><span class="sxs-lookup"><span data-stu-id="6e38b-171">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="6e38b-172">term</span><span class="sxs-lookup"><span data-stu-id="6e38b-172">term</span></span>                 | [<span data-ttu-id="6e38b-173">educationTerm</span><span class="sxs-lookup"><span data-stu-id="6e38b-173">educationTerm</span></span>](../resources/educationterm.md) | <span data-ttu-id="6e38b-174">Termos dessa aula.</span><span class="sxs-lookup"><span data-stu-id="6e38b-174">Term for this class.</span></span>                                               |

## <a name="response"></a><span data-ttu-id="6e38b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e38b-175">Response</span></span>

<span data-ttu-id="6e38b-176">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e38b-176">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e38b-177">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6e38b-177">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e38b-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e38b-178">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

### <a name="response"></a><span data-ttu-id="6e38b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e38b-179">Response</span></span>

> <span data-ttu-id="6e38b-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e38b-180">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
