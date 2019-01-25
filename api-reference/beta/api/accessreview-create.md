---
title: Criar accessReview
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 669b11a8f3b52e867d6b3e803c9419968924928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517796"
---
# <a name="create-accessreview"></a><span data-ttu-id="76c74-103">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="76c74-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c74-104">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="76c74-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="76c74-105">Antes de fazer essa solicitação, o chamador deve ter anteriormente [recuperada a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que o valor de `businessFlowTemplateId` para incluir na solicitação.</span><span class="sxs-lookup"><span data-stu-id="76c74-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="76c74-106">Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md), para vincular a revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="76c74-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="76c74-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="76c74-107">Permissions</span></span>
<span data-ttu-id="76c74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76c74-110">Permission type</span></span>                        | <span data-ttu-id="76c74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76c74-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="76c74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76c74-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76c74-113">AccessReview.ReadWrite.All e também devem ter ProgramControl.ReadWrite.All ao cenário completo com a chamada subsequente para criar um programControl</span><span class="sxs-lookup"><span data-stu-id="76c74-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="76c74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76c74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76c74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76c74-115">Not supported.</span></span> |
|<span data-ttu-id="76c74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76c74-116">Application</span></span>                            | <span data-ttu-id="76c74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76c74-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76c74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76c74-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="76c74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76c74-119">Request headers</span></span>
| <span data-ttu-id="76c74-120">Nome</span><span class="sxs-lookup"><span data-stu-id="76c74-120">Name</span></span>         | <span data-ttu-id="76c74-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="76c74-121">Type</span></span>        | <span data-ttu-id="76c74-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="76c74-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="76c74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76c74-123">Authorization</span></span> | <span data-ttu-id="76c74-124">string</span><span class="sxs-lookup"><span data-stu-id="76c74-124">string</span></span> | <span data-ttu-id="76c74-125">Token de portador</span><span class="sxs-lookup"><span data-stu-id="76c74-125">Bearer \{token\}.</span></span> <span data-ttu-id="76c74-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76c74-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76c74-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76c74-127">Request body</span></span>
<span data-ttu-id="76c74-128">No corpo da solicitação, fornece uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="76c74-128">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="76c74-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria um accessReview.</span><span class="sxs-lookup"><span data-stu-id="76c74-129">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="76c74-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76c74-130">Property</span></span>     | <span data-ttu-id="76c74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76c74-131">Type</span></span>        | <span data-ttu-id="76c74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76c74-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="76c74-133">O nome de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="76c74-133">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="76c74-134">DateTime quando a revisão está agendada para ser iniciar.</span><span class="sxs-lookup"><span data-stu-id="76c74-134">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="76c74-135">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="76c74-135">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="76c74-136">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="76c74-136">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="76c74-137">Isto deve ser de pelo menos um dia mais recente do que a data de início.</span><span class="sxs-lookup"><span data-stu-id="76c74-137">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="76c74-138">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="76c74-138">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="76c74-139">O identificador de modelo de fluxo corporativos, obtido de uma [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="76c74-139">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="76c74-140">O tipo de relacionamento de revisor para os direitos de acesso do objeto revisado, uma das `self`, `delegated`, ou `entityOwners`.</span><span class="sxs-lookup"><span data-stu-id="76c74-140">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="76c74-141">O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="76c74-141">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="76c74-142">Se o reviewerType sendo fornecido tem o valor `delegated`, e em seguida, o chamador também deverá incluir o `reviewers` propriedade, com uma coleção de [userIdentity](../resources/useridentity.md) dos revisores.</span><span class="sxs-lookup"><span data-stu-id="76c74-142">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="76c74-143">Além disso, o chamador pode incluir configurações, para criar uma série recorrente de revisão ou alterar do comportamento padrão de revisão.</span><span class="sxs-lookup"><span data-stu-id="76c74-143">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="76c74-144">Em particular, para criar uma análise mais recorrente, o chamador deve incluir a `accessReviewRecurrenceSettings` dentro do access, revise as configurações,</span><span class="sxs-lookup"><span data-stu-id="76c74-144">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="76c74-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="76c74-145">Response</span></span>
<span data-ttu-id="76c74-146">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76c74-146">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76c74-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76c74-147">Example</span></span>

<span data-ttu-id="76c74-148">Este é um exemplo de criação de uma única (não recorrente) de revisão de acesso, especificando explicitamente os dois usuários como revisores.</span><span class="sxs-lookup"><span data-stu-id="76c74-148">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="76c74-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76c74-149">Request</span></span>
<span data-ttu-id="76c74-150">No corpo da solicitação, fornece uma representação JSON do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="76c74-150">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="76c74-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="76c74-151">Response</span></span>
><span data-ttu-id="76c74-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76c74-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
