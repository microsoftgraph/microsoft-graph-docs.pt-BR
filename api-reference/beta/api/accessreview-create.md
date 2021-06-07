---
title: Criar accessReview
description: No recurso de análises de acesso do Azure AD, crie um novo objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fd1f6c25dcc4013c1abc3d39dafa63723a1e3ea0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751115"
---
# <a name="create-accessreview"></a><span data-ttu-id="9ddea-103">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="9ddea-103">Create accessReview</span></span>

<span data-ttu-id="9ddea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ddea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ddea-105">No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) crie um novo [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="9ddea-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="9ddea-106">Antes de fazer essa solicitação, o chamador deve ter recuperado anteriormente a lista de modelos de fluxo de negócios [,](businessflowtemplate-list.md)para ter o valor **de businessFlowTemplateId** para incluir na solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ddea-106">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of **businessFlowTemplateId** to include in the request.</span></span>

<span data-ttu-id="9ddea-107">Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md), para vincular a revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="9ddea-107">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="9ddea-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ddea-108">Permissions</span></span>

<span data-ttu-id="9ddea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ddea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ddea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ddea-111">Permission type</span></span>                        | <span data-ttu-id="9ddea-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ddea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ddea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ddea-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ddea-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ddea-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9ddea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ddea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ddea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ddea-116">Not supported.</span></span> |
|<span data-ttu-id="9ddea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ddea-117">Application</span></span>                            | <span data-ttu-id="9ddea-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="9ddea-118">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="9ddea-119">O chamador também deve ter permissão ProgramControl.ReadWrite.All, para que depois de criar uma revisão de acesso, o chamador possa criar um [programControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="9ddea-119">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="9ddea-120">Além disso, o usuário inscreveu também deve estar em uma função de diretório que permita que ele crie uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="9ddea-120">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="9ddea-121">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="9ddea-121">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="9ddea-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ddea-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="9ddea-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddea-123">Request headers</span></span>
| <span data-ttu-id="9ddea-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9ddea-124">Name</span></span>         | <span data-ttu-id="9ddea-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ddea-125">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="9ddea-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ddea-126">Authorization</span></span> | <span data-ttu-id="9ddea-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ddea-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="9ddea-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="9ddea-129">Content-type</span></span> | <span data-ttu-id="9ddea-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ddea-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ddea-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddea-132">Request body</span></span>
<span data-ttu-id="9ddea-133">No corpo da solicitação, fornece uma representação JSON de um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="9ddea-133">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="9ddea-134">A tabela a seguir mostra as propriedades que são necessárias ao criar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="9ddea-134">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="9ddea-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ddea-135">Property</span></span>     | <span data-ttu-id="9ddea-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ddea-136">Type</span></span>        | <span data-ttu-id="9ddea-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ddea-137">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ddea-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9ddea-138">displayName</span></span>             |<span data-ttu-id="9ddea-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ddea-139">String</span></span>                                                        | <span data-ttu-id="9ddea-140">O nome da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="9ddea-140">The access review name.</span></span>  |
| <span data-ttu-id="9ddea-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9ddea-141">startDateTime</span></span>           |<span data-ttu-id="9ddea-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ddea-142">DateTimeOffset</span></span>                                                | <span data-ttu-id="9ddea-143">DateTime quando a revisão está agendada para ser inicial.</span><span class="sxs-lookup"><span data-stu-id="9ddea-143">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="9ddea-144">Essa deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="9ddea-144">This must be a date in the future.</span></span>   |
| <span data-ttu-id="9ddea-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9ddea-145">endDateTime</span></span>             |<span data-ttu-id="9ddea-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ddea-146">DateTimeOffset</span></span>                                                | <span data-ttu-id="9ddea-147">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="9ddea-147">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="9ddea-148">Isso deve ser pelo menos um dia depois da data de início.</span><span class="sxs-lookup"><span data-stu-id="9ddea-148">This must be at least one day later than the start date.</span></span>   |
| <span data-ttu-id="9ddea-149">descrição</span><span class="sxs-lookup"><span data-stu-id="9ddea-149">description</span></span>             |<span data-ttu-id="9ddea-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ddea-150">String</span></span>                                                        | <span data-ttu-id="9ddea-151">A descrição, para mostrar aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="9ddea-151">The description, to show to the reviewers.</span></span> |
| <span data-ttu-id="9ddea-152">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="9ddea-152">businessFlowTemplateId</span></span>  |<span data-ttu-id="9ddea-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ddea-153">String</span></span>                                                        | <span data-ttu-id="9ddea-154">O identificador do modelo de fluxo de negócios, obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="9ddea-154">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| <span data-ttu-id="9ddea-155">reviewerType</span><span class="sxs-lookup"><span data-stu-id="9ddea-155">reviewerType</span></span>            |<span data-ttu-id="9ddea-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ddea-156">String</span></span>                                                        | <span data-ttu-id="9ddea-157">O tipo de relação do revistor para os direitos de acesso do objeto revisado, um `self` de `delegated` , ou `entityOwners` .</span><span class="sxs-lookup"><span data-stu-id="9ddea-157">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| <span data-ttu-id="9ddea-158">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="9ddea-158">reviewedEntity</span></span>          |[<span data-ttu-id="9ddea-159">identity</span><span class="sxs-lookup"><span data-stu-id="9ddea-159">identity</span></span>](../resources/identity.md)                                     | <span data-ttu-id="9ddea-160">O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ddea-160">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="9ddea-161">Se o **reviewerType** tiver o valor , o chamador também deverá incluir a propriedade reviewers, com uma coleção de objetos `delegated` [userIdentity](../resources/useridentity.md) representando os revistores. </span><span class="sxs-lookup"><span data-stu-id="9ddea-161">If the **reviewerType** has the value `delegated`, then the caller must also include the **reviewers** property, with a collection of [userIdentity](../resources/useridentity.md) objects representing the reviewers.</span></span>

<span data-ttu-id="9ddea-162">Se seu aplicativo estiver chamando essa API sem um usuário ligado, o chamador também deverá incluir a propriedade **createdBy,** o valor para o qual é uma [userIdentity](../resources/useridentity.md) do usuário que será identificado como o criador da revisão.</span><span class="sxs-lookup"><span data-stu-id="9ddea-162">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="9ddea-163">Além disso, o chamador pode incluir **configurações**, para criar uma série de revisão recorrente ou para alterar do comportamento de revisão padrão.</span><span class="sxs-lookup"><span data-stu-id="9ddea-163">In addition, the caller can include **settings**, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="9ddea-164">Em particular, para criar uma revisão recorrente, o chamador deve incluir [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) dentro das configurações de revisão de acesso,</span><span class="sxs-lookup"><span data-stu-id="9ddea-164">In particular, to create a recurring review, the caller must include the [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="9ddea-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ddea-165">Response</span></span>
<span data-ttu-id="9ddea-166">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ddea-166">If successful, this method returns a `201 Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ddea-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ddea-167">Example</span></span>

<span data-ttu-id="9ddea-168">Este é um exemplo de criação de uma revisão de acesso única (não recorrente), especificando explicitamente dois usuários como revistores.</span><span class="sxs-lookup"><span data-stu-id="9ddea-168">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

### <a name="request"></a><span data-ttu-id="9ddea-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ddea-169">Request</span></span>
<span data-ttu-id="9ddea-170">No corpo da solicitação, fornece uma representação JSON do [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="9ddea-170">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ddea-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ddea-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="9ddea-172">C#</span><span class="sxs-lookup"><span data-stu-id="9ddea-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ddea-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ddea-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ddea-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ddea-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ddea-175">Java</span><span class="sxs-lookup"><span data-stu-id="9ddea-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ddea-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ddea-176">Response</span></span>
><span data-ttu-id="9ddea-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9ddea-177">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


