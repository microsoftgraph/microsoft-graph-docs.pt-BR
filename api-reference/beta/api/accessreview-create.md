---
title: Criar accessReview
description: No recurso de revisões do Azure AD Access, crie um novo objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fe636c531ba4a9b82c44427002937876c8e4178
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172772"
---
# <a name="create-accessreview"></a><span data-ttu-id="de154-103">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="de154-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de154-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="de154-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="de154-105">Antes de fazer essa solicitação, o chamador deve ter [recuperado previamente a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que `businessFlowTemplateId` o valor de seja incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="de154-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="de154-106">Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md)para vincular a revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="de154-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="de154-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="de154-107">Permissions</span></span>
<span data-ttu-id="de154-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de154-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de154-110">Permission type</span></span>                        | <span data-ttu-id="de154-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de154-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="de154-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de154-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de154-113">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="de154-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="de154-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de154-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de154-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de154-115">Not supported.</span></span> |
|<span data-ttu-id="de154-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de154-116">Application</span></span>                            | <span data-ttu-id="de154-117">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="de154-117">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="de154-118">O chamador também deve ter a permissão ProgramControl. ReadWrite. All, de modo que depois de criar uma revisão do Access, o chamador possa criar um [ProgramControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="de154-118">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="de154-119">Além disso, o usuário conectado também deve estar em uma função de diretório que permite que eles criem uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="de154-119">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="de154-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="de154-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="de154-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de154-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="de154-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de154-122">Request headers</span></span>
| <span data-ttu-id="de154-123">Nome</span><span class="sxs-lookup"><span data-stu-id="de154-123">Name</span></span>         | <span data-ttu-id="de154-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="de154-124">Type</span></span>        | <span data-ttu-id="de154-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="de154-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="de154-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="de154-126">Authorization</span></span> | <span data-ttu-id="de154-127">string</span><span class="sxs-lookup"><span data-stu-id="de154-127">string</span></span> | <span data-ttu-id="de154-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de154-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de154-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de154-130">Request body</span></span>
<span data-ttu-id="de154-131">No corpo da solicitação, forneça uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="de154-131">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="de154-132">A tabela a seguir mostra as propriedades que são necessárias ao criar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="de154-132">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="de154-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de154-133">Property</span></span>     | <span data-ttu-id="de154-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="de154-134">Type</span></span>        | <span data-ttu-id="de154-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="de154-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="de154-136">O nome de revisão do acesso.</span><span class="sxs-lookup"><span data-stu-id="de154-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="de154-137">O DateTime quando a revisão está agendada para ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="de154-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="de154-138">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="de154-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="de154-139">O DateTime quando a revisão é agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="de154-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="de154-140">Este deve ser pelo menos um dia depois da data de início.</span><span class="sxs-lookup"><span data-stu-id="de154-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="de154-141">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="de154-141">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="de154-142">O identificador do modelo de fluxo de negócios obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="de154-142">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="de154-143">O tipo de relação de revisor para os direitos de acesso do objeto revisado, `self`um `delegated`de, `entityOwners`ou.</span><span class="sxs-lookup"><span data-stu-id="de154-143">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="de154-144">O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de154-144">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="de154-145">Se o revisortype que está sendo fornecido tiver `delegated`o valor, o chamador também deverá incluir `reviewers` a propriedade, com uma coleção de UserIdentity dos revisores. [](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="de154-145">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="de154-146">Se seu aplicativo estiver chamando esta API sem um usuário conectado, o chamador também deverá incluir a propriedade **createdBy** , o valor para o qual é um UserIdentity [](../resources/useridentity.md) do usuário que será identificado como criador da revisão.</span><span class="sxs-lookup"><span data-stu-id="de154-146">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="de154-147">Além disso, o chamador pode incluir configurações, para criar uma série de análise recorrente ou para alterar o comportamento de revisão padrão.</span><span class="sxs-lookup"><span data-stu-id="de154-147">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="de154-148">Em particular, para criar uma revisão recorrente, o chamador deve incluir as `accessReviewRecurrenceSettings` configurações de revisão do Access,</span><span class="sxs-lookup"><span data-stu-id="de154-148">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="de154-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="de154-149">Response</span></span>
<span data-ttu-id="de154-150">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de154-150">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de154-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de154-151">Example</span></span>

<span data-ttu-id="de154-152">Este é um exemplo de criação de uma revisão de acesso de uma única vez (não recorrente), especificando explicitamente dois usuários como os revisores.</span><span class="sxs-lookup"><span data-stu-id="de154-152">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="de154-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de154-153">Request</span></span>
<span data-ttu-id="de154-154">No corpo da solicitação, forneça uma representação JSON do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="de154-154">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de154-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="de154-155">HTTP</span></span>](#tab/http)
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
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="de154-156">C#</span><span class="sxs-lookup"><span data-stu-id="de154-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de154-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="de154-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de154-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de154-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="de154-159">Java</span><span class="sxs-lookup"><span data-stu-id="de154-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de154-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="de154-160">Response</span></span>
><span data-ttu-id="de154-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de154-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
