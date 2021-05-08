---
title: Criar accessReviewHistoryDefinition
description: Crie um novo objeto accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1ecb35c0c56d0db937aca60fa00d3559f0a063c4
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232890"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="529f1-103">Criar accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="529f1-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="529f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="529f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="529f1-105">Crie um novo [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="529f1-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="529f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="529f1-106">Permissions</span></span>

<span data-ttu-id="529f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="529f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="529f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="529f1-109">Permission type</span></span>|<span data-ttu-id="529f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="529f1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="529f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="529f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="529f1-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529f1-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="529f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="529f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="529f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="529f1-114">Not supported.</span></span>|
|<span data-ttu-id="529f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="529f1-115">Application</span></span>|<span data-ttu-id="529f1-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529f1-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="529f1-117">O usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso para recuperar todos os dados.</span><span class="sxs-lookup"><span data-stu-id="529f1-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="529f1-118">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="529f1-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="529f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="529f1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="529f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="529f1-120">Request headers</span></span>

|<span data-ttu-id="529f1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="529f1-121">Name</span></span>|<span data-ttu-id="529f1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="529f1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="529f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="529f1-123">Authorization</span></span>|<span data-ttu-id="529f1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="529f1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="529f1-126">Content-Type</span></span>|<span data-ttu-id="529f1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="529f1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="529f1-129">Request body</span></span>

<span data-ttu-id="529f1-130">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="529f1-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="529f1-131">A tabela a seguir mostra as propriedades necessárias usadas para criar [um accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="529f1-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="529f1-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="529f1-132">Property</span></span>|<span data-ttu-id="529f1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="529f1-133">Type</span></span>|<span data-ttu-id="529f1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="529f1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="529f1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="529f1-135">displayName</span></span> | <span data-ttu-id="529f1-136">String</span><span class="sxs-lookup"><span data-stu-id="529f1-136">String</span></span>  | <span data-ttu-id="529f1-137">Nome da coleção de dados do histórico de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="529f1-137">Name for the access review history data collection.</span></span> <span data-ttu-id="529f1-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-138">Required.</span></span> |
|<span data-ttu-id="529f1-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="529f1-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="529f1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529f1-140">DateTimeOffset</span></span>  | <span data-ttu-id="529f1-141">Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="529f1-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="529f1-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-142">Required.</span></span>  |
|<span data-ttu-id="529f1-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="529f1-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="529f1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529f1-144">DateTimeOffset</span></span>  | <span data-ttu-id="529f1-145">Timestamp, as avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="529f1-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="529f1-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-146">Required.</span></span>  |
|<span data-ttu-id="529f1-147">escopos</span><span class="sxs-lookup"><span data-stu-id="529f1-147">scopes</span></span>|<span data-ttu-id="529f1-148">coleção microsoft.graph.accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="529f1-148">microsoft.graph.accessReviewQueryScope collection</span></span>| <span data-ttu-id="529f1-149">Usado para filtrar quais avaliações estão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="529f1-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="529f1-150">Busca avaliações cujo escopo corresponde a esse escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="529f1-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="529f1-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="529f1-151">Required.</span></span>  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="529f1-152">Consultas de escopo com suporte para accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="529f1-152">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="529f1-153">A seguir, há consultas com suporte em [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) com base no [accessreviewqueryscope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="529f1-153">The following are queries supported on an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) based on the [accessreviewqueryscope](../resources/accessreviewqueryscope.md).</span></span> <span data-ttu-id="529f1-154">Esses escopos ditam que tipo de dados de histórico de revisão são incluídos no arquivo CSV baixável gerado quando a definição é criada.</span><span class="sxs-lookup"><span data-stu-id="529f1-154">These scopes dictate which type of review history data is included in the downloadable CSV file which is generated when the definition is created.</span></span>

|<span data-ttu-id="529f1-155">Cenário</span><span class="sxs-lookup"><span data-stu-id="529f1-155">Scenario</span></span>| <span data-ttu-id="529f1-156">Consulta</span><span class="sxs-lookup"><span data-stu-id="529f1-156">Query</span></span> |
|--|--|
| <span data-ttu-id="529f1-157">Incluir cada resultado de revisão em grupos individuais (exclui definições com escopo para todos os grupos Microsoft 365 `accessReviewScheduleDefinition` com usuários convidados)</span><span class="sxs-lookup"><span data-stu-id="529f1-157">Include every `accessReviewScheduleDefinition` review result on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="529f1-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span><span class="sxs-lookup"><span data-stu-id="529f1-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span></span> |
| <span data-ttu-id="529f1-159">Incluir todos os resultados de revisão em um grupo específico (exclui definições com escopo para todos os grupos Microsoft 365 `accessReviewScheduleDefinition` com usuários convidados)</span><span class="sxs-lookup"><span data-stu-id="529f1-159">Include every `accessReviewScheduleDefinition` review result on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="529f1-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span><span class="sxs-lookup"><span data-stu-id="529f1-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span></span> |
| <span data-ttu-id="529f1-161">Incluir todos `accessReviewScheduleDefinition` os resultados de revisão com escopo para todos os grupos Microsoft 365 com usuários convidados</span><span class="sxs-lookup"><span data-stu-id="529f1-161">Include every `accessReviewScheduleDefinition` review result scoped to all Microsoft 365 groups with guest users</span></span> | <span data-ttu-id="529f1-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span><span class="sxs-lookup"><span data-stu-id="529f1-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span></span> |
| <span data-ttu-id="529f1-163">Incluir todos `accessReviewScheduleDefinition` os resultados de revisão em um pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="529f1-163">Include every `accessReviewScheduleDefinition` review result on an access package</span></span> | <span data-ttu-id="529f1-164">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')</span><span class="sxs-lookup"><span data-stu-id="529f1-164">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')</span></span> |
| <span data-ttu-id="529f1-165">Incluir todos `accessReviewScheduleDefinition` os resultados de revisão para entidades de serviço atribuídas à função privilegiada</span><span class="sxs-lookup"><span data-stu-id="529f1-165">Include every `accessReviewScheduleDefinition` review result for service principals assigned to privileged role</span></span> | <span data-ttu-id="529f1-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span><span class="sxs-lookup"><span data-stu-id="529f1-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span></span> |
| <span data-ttu-id="529f1-167">Incluir cada `accessReviewScheduleDefinition` resultado de revisão para reivews de um grupo específico</span><span class="sxs-lookup"><span data-stu-id="529f1-167">Include every `accessReviewScheduleDefinition` review result for reivews of a specific group</span></span> | <span data-ttu-id="529f1-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span><span class="sxs-lookup"><span data-stu-id="529f1-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span></span> |

## <a name="response"></a><span data-ttu-id="529f1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="529f1-169">Response</span></span>

<span data-ttu-id="529f1-170">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="529f1-170">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="529f1-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="529f1-171">Examples</span></span>

<span data-ttu-id="529f1-172">O exemplo a seguir mostra como criar uma definição de histórico de revisão de acesso com escopo para acessar análises em pacotes e grupos de acesso, em execução entre a data de início de 01/01/2021 e a data de término de 05/04/2021.</span><span class="sxs-lookup"><span data-stu-id="529f1-172">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="529f1-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="529f1-173">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="529f1-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="529f1-174">Response</span></span>
><span data-ttu-id="529f1-175">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="529f1-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
