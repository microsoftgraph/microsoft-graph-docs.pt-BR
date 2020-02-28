---
title: Criar accessReview
description: No recurso de revisões do Azure AD Access, crie um novo objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae1730d2d7cea0d5cb36e13c25d1c2b550d42a0d
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331161"
---
# <a name="create-accessreview"></a><span data-ttu-id="301fb-103">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="301fb-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="301fb-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="301fb-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="301fb-105">Antes de fazer essa solicitação, o chamador deve ter [recuperado previamente a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que `businessFlowTemplateId` o valor de seja incluído na solicitação.</span><span class="sxs-lookup"><span data-stu-id="301fb-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="301fb-106">Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md)para vincular a revisão do Access a um programa.</span><span class="sxs-lookup"><span data-stu-id="301fb-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="301fb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="301fb-107">Permissions</span></span>

<span data-ttu-id="301fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="301fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="301fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="301fb-110">Permission type</span></span>                        | <span data-ttu-id="301fb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="301fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="301fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="301fb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="301fb-113">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="301fb-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="301fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="301fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="301fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="301fb-115">Not supported.</span></span> |
|<span data-ttu-id="301fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="301fb-116">Application</span></span>                            | <span data-ttu-id="301fb-117">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="301fb-117">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="301fb-118">O chamador também deve ter a permissão ProgramControl. ReadWrite. All, de modo que depois de criar uma revisão do Access, o chamador possa criar um [ProgramControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="301fb-118">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="301fb-119">Além disso, o usuário conectado também deve estar em uma função de diretório que permite que eles criem uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="301fb-119">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="301fb-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="301fb-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="301fb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="301fb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="301fb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="301fb-122">Request headers</span></span>
| <span data-ttu-id="301fb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="301fb-123">Name</span></span>         | <span data-ttu-id="301fb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="301fb-124">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="301fb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="301fb-125">Authorization</span></span> | <span data-ttu-id="301fb-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="301fb-126">Bearer \{token\}.</span></span> <span data-ttu-id="301fb-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="301fb-127">Required.</span></span> |
| <span data-ttu-id="301fb-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="301fb-128">Content-type</span></span> | <span data-ttu-id="301fb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="301fb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="301fb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="301fb-131">Request body</span></span>
<span data-ttu-id="301fb-132">No corpo da solicitação, forneça uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="301fb-132">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="301fb-133">A tabela a seguir mostra as propriedades que são necessárias ao criar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="301fb-133">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="301fb-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="301fb-134">Property</span></span>     | <span data-ttu-id="301fb-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="301fb-135">Type</span></span>        | <span data-ttu-id="301fb-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="301fb-136">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="301fb-137">O nome de revisão do acesso.</span><span class="sxs-lookup"><span data-stu-id="301fb-137">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="301fb-138">O DateTime quando a revisão está agendada para ser iniciada.</span><span class="sxs-lookup"><span data-stu-id="301fb-138">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="301fb-139">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="301fb-139">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="301fb-140">O DateTime quando a revisão é agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="301fb-140">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="301fb-141">Este deve ser pelo menos um dia depois da data de início.</span><span class="sxs-lookup"><span data-stu-id="301fb-141">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="301fb-142">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="301fb-142">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="301fb-143">O identificador do modelo de fluxo de negócios obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="301fb-143">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="301fb-144">O tipo de relação de revisor para os direitos de acesso do objeto revisado, `self`um `delegated`de, `entityOwners`ou.</span><span class="sxs-lookup"><span data-stu-id="301fb-144">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="301fb-145">O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="301fb-145">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="301fb-146">Se o revisortype que está sendo fornecido tiver `delegated`o valor, o chamador também deverá incluir `reviewers` a propriedade, com uma coleção de [UserIdentity](../resources/useridentity.md) dos revisores.</span><span class="sxs-lookup"><span data-stu-id="301fb-146">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="301fb-147">Se seu aplicativo estiver chamando esta API sem um usuário conectado, o chamador também deverá incluir a propriedade **createdBy** , o valor para o qual é um [UserIdentity](../resources/useridentity.md) do usuário que será identificado como criador da revisão.</span><span class="sxs-lookup"><span data-stu-id="301fb-147">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="301fb-148">Além disso, o chamador pode incluir configurações, para criar uma série de análise recorrente ou para alterar o comportamento de revisão padrão.</span><span class="sxs-lookup"><span data-stu-id="301fb-148">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="301fb-149">Em particular, para criar uma revisão recorrente, o chamador deve incluir as `accessReviewRecurrenceSettings` configurações de revisão do Access,</span><span class="sxs-lookup"><span data-stu-id="301fb-149">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="301fb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="301fb-150">Response</span></span>
<span data-ttu-id="301fb-151">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="301fb-151">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="301fb-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="301fb-152">Example</span></span>

<span data-ttu-id="301fb-153">Este é um exemplo de criação de uma revisão de acesso de uma única vez (não recorrente), especificando explicitamente dois usuários como os revisores.</span><span class="sxs-lookup"><span data-stu-id="301fb-153">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

### <a name="request"></a><span data-ttu-id="301fb-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="301fb-154">Request</span></span>
<span data-ttu-id="301fb-155">No corpo da solicitação, forneça uma representação JSON do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="301fb-155">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "ignored",
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

### <a name="response"></a><span data-ttu-id="301fb-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="301fb-156">Response</span></span>
><span data-ttu-id="301fb-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="301fb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
