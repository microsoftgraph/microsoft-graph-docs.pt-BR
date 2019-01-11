---
title: Criar accessReview
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto accessReview.
localization_priority: Normal
ms.openlocfilehash: 1ee5ce696f1d71c57adf9e6c5ee30c067536c8ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851440"
---
# <a name="create-accessreview"></a><span data-ttu-id="c0662-103">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="c0662-103">Create accessReview</span></span>

> <span data-ttu-id="c0662-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0662-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0662-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0662-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0662-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="c0662-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c0662-107">Antes de fazer essa solicitação, o chamador deve ter anteriormente [recuperada a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que o valor de `businessFlowTemplateId` para incluir na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0662-107">Prior to making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="c0662-108">Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md), para vincular a revisão de acesso a um programa.</span><span class="sxs-lookup"><span data-stu-id="c0662-108">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c0662-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="c0662-109">Permissions</span></span>
<span data-ttu-id="c0662-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0662-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0662-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0662-112">Permission type</span></span>                        | <span data-ttu-id="c0662-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0662-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0662-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0662-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0662-115">AccessReview.ReadWrite.All e também devem ter ProgramControl.ReadWrite.All ao cenário completo com a chamada subsequente para criar um programControl</span><span class="sxs-lookup"><span data-stu-id="c0662-115">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="c0662-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0662-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0662-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0662-117">Not supported.</span></span> |
|<span data-ttu-id="c0662-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0662-118">Application</span></span>                            | <span data-ttu-id="c0662-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0662-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0662-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0662-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="c0662-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0662-121">Request headers</span></span>
| <span data-ttu-id="c0662-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c0662-122">Name</span></span>         | <span data-ttu-id="c0662-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0662-123">Type</span></span>        | <span data-ttu-id="c0662-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0662-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c0662-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0662-125">Authorization</span></span> | <span data-ttu-id="c0662-126">string</span><span class="sxs-lookup"><span data-stu-id="c0662-126">string</span></span> | <span data-ttu-id="c0662-127">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="c0662-127">Bearer \{token\}.</span></span> <span data-ttu-id="c0662-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0662-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0662-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0662-129">Request body</span></span>
<span data-ttu-id="c0662-130">No corpo da solicitação, fornece uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="c0662-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="c0662-131">A tabela a seguir mostra as propriedades que são necessárias quando você cria um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c0662-131">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="c0662-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0662-132">Property</span></span>     | <span data-ttu-id="c0662-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0662-133">Type</span></span>        | <span data-ttu-id="c0662-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0662-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="c0662-135">O nome de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="c0662-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="c0662-136">DateTime quando a revisão está agendada para ser iniciar.</span><span class="sxs-lookup"><span data-stu-id="c0662-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="c0662-137">Isso deve ser uma data no futuro.</span><span class="sxs-lookup"><span data-stu-id="c0662-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="c0662-138">DateTime quando a revisão está agendada para terminar.</span><span class="sxs-lookup"><span data-stu-id="c0662-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="c0662-139">Isto deve ser de pelo menos um dia mais recente do que a data de início.</span><span class="sxs-lookup"><span data-stu-id="c0662-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="c0662-140">A descrição, para mostrar aos revisores.</span><span class="sxs-lookup"><span data-stu-id="c0662-140">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="c0662-141">O identificador de modelo de fluxo corporativos, obtido de uma [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0662-141">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="c0662-142">O tipo de relacionamento de revisor para os direitos de acesso do objeto revisado, uma das `self`, `delegate` ou `entityOwners`.</span><span class="sxs-lookup"><span data-stu-id="c0662-142">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegate` or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="c0662-143">O objeto para o qual uma revisão de acesso é criada, como um associações de um grupo ou as atribuições de usuários para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c0662-143">The object for which an access review is created, such as a memberships of an group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="c0662-144">Se o reviewerType sendo fornecido tem o valor `delegate`, e em seguida, o chamador também deverá incluir o `reviewers` propriedade, com uma coleção de [userIdentity](../resources/useridentity.md) dos revisores.</span><span class="sxs-lookup"><span data-stu-id="c0662-144">If the reviewerType being supplied has the value `delegate`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="c0662-145">Além disso, o chamador pode incluir configurações, para criar uma série recorrente de revisão ou alterar do comportamento padrão de revisão.</span><span class="sxs-lookup"><span data-stu-id="c0662-145">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="c0662-146">Em particular, para criar uma análise mais recorrente, o chamador deve incluir a `accessReviewRecurrenceSettings` dentro do access, revise as configurações,</span><span class="sxs-lookup"><span data-stu-id="c0662-146">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="c0662-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0662-147">Response</span></span>
<span data-ttu-id="c0662-148">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0662-148">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0662-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0662-149">Example</span></span>

<span data-ttu-id="c0662-150">Este é um exemplo de criação de uma única (não recorrente) de revisão de acesso, especificando explicitamente os dois usuários como revisores.</span><span class="sxs-lookup"><span data-stu-id="c0662-150">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="c0662-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0662-151">Request</span></span>
<span data-ttu-id="c0662-152">No corpo da solicitação, fornece uma representação JSON do objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="c0662-152">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

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
    "reviewerType" : "delegate",
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
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
    }
}
```

##### <a name="response"></a><span data-ttu-id="c0662-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0662-153">Response</span></span>
><span data-ttu-id="c0662-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0662-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
