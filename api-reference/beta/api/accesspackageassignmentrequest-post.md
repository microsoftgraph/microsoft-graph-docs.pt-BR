---
title: Criar accessPackageAssignmentRequest
description: Crie um novo accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d455bde8192cfd37713d32f10e5bb8d8b908cec0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868872"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="9cc7e-103">Criar accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9cc7e-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="9cc7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc7e-105">No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), crie um novo [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9cc7e-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="9cc7e-106">Essa operação é usada para atribuir um usuário a um pacote de acesso ou para remover uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc7e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9cc7e-107">Permissions</span></span>

<span data-ttu-id="9cc7e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cc7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc7e-110">Permission type</span></span>                        | <span data-ttu-id="9cc7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cc7e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9cc7e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc7e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cc7e-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc7e-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9cc7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-115">Not supported.</span></span> |
| <span data-ttu-id="9cc7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc7e-116">Application</span></span>                            | <span data-ttu-id="9cc7e-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc7e-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc7e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="9cc7e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-119">Request headers</span></span>

| <span data-ttu-id="9cc7e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9cc7e-120">Name</span></span>          | <span data-ttu-id="9cc7e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc7e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9cc7e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc7e-122">Authorization</span></span> | <span data-ttu-id="9cc7e-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="9cc7e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cc7e-125">Content-Type</span></span>  | <span data-ttu-id="9cc7e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc7e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-128">Request body</span></span>

<span data-ttu-id="9cc7e-129">No corpo da solicitação, fornece uma representação JSON [do objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9cc7e-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="9cc7e-130">Para que um administrador solicite a criação de uma atribuição para um usuário, o valor da propriedade **requestType** é , e a propriedade accessPackageAssignment contém o do usuário que está sendo atribuído, a propriedade `AdminAdd`  `targetId` **assignmentPolicyId** que identifica [o accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)e a propriedade **accessPackageId** que identifica [o accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-130">For an administrator to request to create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="9cc7e-131">Para que um administrador solicite a remoção de uma atribuição, o valor da propriedade **requestType** é , e a propriedade `AdminRemove` **accessPackageAssignment** contém a propriedade **id** que identifica [o accessPackageAssignment](../resources/accesspackageassignment.md) sendo removido.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-131">For an administrator to request to remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

<span data-ttu-id="9cc7e-132">Para um usuário não administrador solicitar a criação de sua própria atribuição para uma primeira atribuição ou renovação de atribuição, o valor da **propriedade requestType** é `UserAdd` .</span><span class="sxs-lookup"><span data-stu-id="9cc7e-132">For a non-administrator user to request to create their own assignment for either a first assignment or renew assignment, the value of the **requestType** property is `UserAdd`.</span></span> <span data-ttu-id="9cc7e-133">A **propriedade accessPackageAssignment** contém `targetId` a com os `id` usuários.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-133">The **accessPackageAssignment** property contains the `targetId` with the `id` of the users.</span></span> <span data-ttu-id="9cc7e-134">A **propriedade assignmentPolicyId** identifica [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-134">The **assignmentPolicyId** property identifies the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9cc7e-135">A **propriedade accessPackageId** identifica [o accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-135">The **accessPackageId** property identifies the [accessPackage](../resources/accesspackage.md).</span></span> <span data-ttu-id="9cc7e-136">O usuário que faz a solicitação já deve existir no diretório.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-136">The user making the request must already exist in the directory.</span></span>

<span data-ttu-id="9cc7e-137">Para um usuário que não seja administrador solicitar estender suas próprias atribuições, o valor da **propriedade requestType** é `UserExtend` .</span><span class="sxs-lookup"><span data-stu-id="9cc7e-137">For a non-administrator user to request to extend their own assignments, the value of the **requestType** property is `UserExtend`.</span></span> <span data-ttu-id="9cc7e-138">A **propriedade accessPackageAssignment** contém `targetId` a com os `id` usuários.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-138">The **accessPackageAssignment** property contains the `targetId` with the `id` of the users.</span></span> <span data-ttu-id="9cc7e-139">A **propriedade assignmentPolicyId** identifica [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-139">The **assignmentPolicyId** property identifies the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9cc7e-140">A **propriedade accessPackageId** identifica [o accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-140">The **accessPackageId** property identifies the [accessPackage](../resources/accesspackage.md).</span></span> <span data-ttu-id="9cc7e-141">O usuário que faz a solicitação já deve existir no diretório.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-141">The user making the request must already exist in the directory.</span></span>

## <a name="response"></a><span data-ttu-id="9cc7e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7e-142">Response</span></span>

<span data-ttu-id="9cc7e-143">Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-143">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  

<span data-ttu-id="9cc7e-144">Se isso for uma solicitação, em seguida, um `AdminAdd` [accessPackageAssignment](../resources/accesspackageassignment.md) e, se necessário, um [accessPackageSubject](../resources/accesspackagesubject.md) também serão criados.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-144">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="9cc7e-145">Você pode localizá-los usando os parâmetros de consulta ao [listar accessPackageAssignments](accesspackageassignment-list.md).</span><span class="sxs-lookup"><span data-stu-id="9cc7e-145">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="9cc7e-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9cc7e-146">Examples</span></span>
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a><span data-ttu-id="9cc7e-147">Exemplo 1: o administrador solicita uma atribuição direta para um usuário</span><span class="sxs-lookup"><span data-stu-id="9cc7e-147">Example 1: Admin requests a direct assignment for a user</span></span>
#### <a name="request"></a><span data-ttu-id="9cc7e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-148">Request</span></span>

<span data-ttu-id="9cc7e-149">A seguir está um exemplo da solicitação de uma atribuição direta, na qual o administrador está solicitando a criação de uma atribuição para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-149">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="9cc7e-150">Como o [accessPackageSubject](../resources/accesspackagesubject.md) pode ainda não existir, o valor do **targetID** é a ID do objeto do usuário que está sendo atribuído, o valor do **accessPackageId** é o pacote de acesso desejado para esse usuário, e o valor de **assignmentPolicyId** é uma política de atribuição direta nesse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-150">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="9cc7e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc7e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9cc7e-152">C#</span><span class="sxs-lookup"><span data-stu-id="9cc7e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc7e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc7e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc7e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc7e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc7e-155">Java</span><span class="sxs-lookup"><span data-stu-id="9cc7e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc7e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7e-156">Response</span></span>

<span data-ttu-id="9cc7e-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-157">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc7e-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a><span data-ttu-id="9cc7e-159">Exemplo 2: o usuário solicita um pacote e responde perguntas para aprovação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-159">Example 2: User requests a package and answers questions for approval</span></span>
#### <a name="request"></a><span data-ttu-id="9cc7e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-160">Request</span></span>

<span data-ttu-id="9cc7e-161">A seguir, um exemplo de uma solicitação em que o solicitante forneceu respostas ao aprovador para ajudá-lo a tomar sua decisão.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-161">The following is an example of a request where the requestor provided answers to the approver to help them make their decision.</span></span>
 



# <a name="http"></a>[<span data-ttu-id="9cc7e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc7e-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
        "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
        }
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="9cc7e-163">C#</span><span class="sxs-lookup"><span data-stu-id="9cc7e-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc7e-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc7e-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc7e-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc7e-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cc7e-166">Java</span><span class="sxs-lookup"><span data-stu-id="9cc7e-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="9cc7e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7e-167">Response</span></span>

<span data-ttu-id="9cc7e-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-168">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc7e-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e382d02-4454-436b-b700-59c7dd77f466",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
            "isRequired": false,
            "text": {
                "defaultText": "what state are you from?",
                "localizedTexts": [{
                    "text": "¿De qué estado eres?",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
            "choices": [{
                "actualValue": "AZ",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Arizona",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "CA",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "California",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "OH",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Ohio",
                        "languageCode": "es"
                    }]
                }
            }],
            "allowsMultipleSelection": false
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
            "isRequired": false,
            "text": {
                "defaultText": "Who is your manager?",
                "localizedTexts": [{
                    "text": "por qué necesita acceso a este paquete",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": false
        }
    }]
}
```
### <a name="example-3-request-a-package-and-provide-a-justification"></a><span data-ttu-id="9cc7e-170">Exemplo 3: solicitar um pacote e fornecer uma justificativa</span><span class="sxs-lookup"><span data-stu-id="9cc7e-170">Example 3: Request a package and provide a justification</span></span>
#### <a name="request"></a><span data-ttu-id="9cc7e-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-171">Request</span></span>

<span data-ttu-id="9cc7e-172">O exemplo a seguir mostra como solicitar um pacote de acesso e fornecer justificativa ao aprovador.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-172">The following example shows how to request an access package and provide justification to the approver.</span></span>
 


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "justification":"Need access to New Hire access package"
}
```

#### <a name="response"></a><span data-ttu-id="9cc7e-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7e-173">Response</span></span>

<span data-ttu-id="9cc7e-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-174">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc7e-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "813bbc6b-31f5-4cdf-8fed-1ba4284a1e3f",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": "Requested for the new task.",
    "answers": [],
    "schedule": {
        "startDateTime": null,
        "recurrence": null,
        "expiration": {
            "endDateTime": null,
            "duration": null,
            "type": null
        }
    }
}
```

### <a name="example-4-remove-an-assignment"></a><span data-ttu-id="9cc7e-177">Exemplo 4: Remover uma atribuição</span><span class="sxs-lookup"><span data-stu-id="9cc7e-177">Example 4: Remove an assignment</span></span>

<span data-ttu-id="9cc7e-178">Para remover atribuições, crie um novo objeto accessPackageAssignmentRequest com as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="9cc7e-178">To remove assignments, create a new accessPackageAssignmentRequest object with the following settings:</span></span>

+ <span data-ttu-id="9cc7e-179">O valor da **propriedade requestType** definida como `AdminRemove` .</span><span class="sxs-lookup"><span data-stu-id="9cc7e-179">The value of the **requestType** property set to `AdminRemove`.</span></span>
+ <span data-ttu-id="9cc7e-180">Na propriedade accessPackageAssignment, inclua uma lista com o identificador dos objetos accessPackageAssignment a ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-180">In the accessPackageAssignment property, include a list with the identifier of the accessPackageAssignment objects to delete.</span></span>

#### <a name="request"></a><span data-ttu-id="9cc7e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc7e-181">Request</span></span>

<span data-ttu-id="9cc7e-182">O exemplo a seguir mostra como remover uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-182">The following example shows how to remove an assignment.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "AdminRemove",
    "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
}
```

#### <a name="response"></a><span data-ttu-id="9cc7e-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc7e-183">Response</span></span>

<span data-ttu-id="9cc7e-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-184">The following is an example of the response.</span></span>

> <span data-ttu-id="9cc7e-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc7e-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


