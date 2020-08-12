---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: b6b3ca4865e56961f6388e9be1a567de73026472
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643992"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="fb1dc-103">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-103">agreement resource type</span></span>

<span data-ttu-id="fb1dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb1dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb1dc-105">Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fb1dc-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="fb1dc-106">Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="fb1dc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb1dc-107">Methods</span></span>

| <span data-ttu-id="fb1dc-108">Método</span><span class="sxs-lookup"><span data-stu-id="fb1dc-108">Method</span></span>       | <span data-ttu-id="fb1dc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb1dc-109">Return Type</span></span> | <span data-ttu-id="fb1dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb1dc-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fb1dc-111">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="fb1dc-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="fb1dc-112">contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-112">agreement</span></span>](agreement.md) | <span data-ttu-id="fb1dc-113">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="fb1dc-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="fb1dc-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="fb1dc-115">coleção de [contratos](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="fb1dc-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="fb1dc-116">Obtenha uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="fb1dc-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="fb1dc-118">contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-118">agreement</span></span>](agreement.md) | <span data-ttu-id="fb1dc-119">Leia as propriedades e as relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="fb1dc-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="fb1dc-121">contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-121">agreement</span></span>](agreement.md) | <span data-ttu-id="fb1dc-122">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="fb1dc-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="fb1dc-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="fb1dc-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb1dc-124">None</span></span> | <span data-ttu-id="fb1dc-125">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="fb1dc-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb1dc-126">Properties</span></span>
| <span data-ttu-id="fb1dc-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb1dc-127">Property</span></span>     | <span data-ttu-id="fb1dc-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb1dc-128">Type</span></span>        | <span data-ttu-id="fb1dc-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb1dc-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb1dc-130">displayName</span><span class="sxs-lookup"><span data-stu-id="fb1dc-130">displayName</span></span>|<span data-ttu-id="fb1dc-131">String</span><span class="sxs-lookup"><span data-stu-id="fb1dc-131">String</span></span>|<span data-ttu-id="fb1dc-132">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-132">Display name of the agreement.</span></span> <span data-ttu-id="fb1dc-133">O nome para exibição é usado para o controle interno do contrato, mas não é exibido para os usuários finais que exibem o contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="fb1dc-134">id</span><span class="sxs-lookup"><span data-stu-id="fb1dc-134">id</span></span>|<span data-ttu-id="fb1dc-135">String</span><span class="sxs-lookup"><span data-stu-id="fb1dc-135">String</span></span>| <span data-ttu-id="fb1dc-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-136">Read-only.</span></span>|
|<span data-ttu-id="fb1dc-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="fb1dc-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="fb1dc-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb1dc-138">Boolean</span></span>|<span data-ttu-id="fb1dc-139">Essa configuração permite que você exija que os usuários finais aceitem este contrato em todos os dispositivos dos quais eles estão acessando-os.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="fb1dc-140">O usuário final será solicitado a registrar o dispositivo no Azure AD, caso ainda não tenha feito isso.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="fb1dc-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="fb1dc-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="fb1dc-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb1dc-142">Boolean</span></span>|<span data-ttu-id="fb1dc-143">Indica se o usuário tem que expandir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="fb1dc-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="fb1dc-144">termsExpiration</span></span>|[<span data-ttu-id="fb1dc-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="fb1dc-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="fb1dc-146">Cronograma de expiração e frequência de contrato para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="fb1dc-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="fb1dc-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="fb1dc-148">Duração</span><span class="sxs-lookup"><span data-stu-id="fb1dc-148">Duration</span></span>|<span data-ttu-id="fb1dc-149">A duração após a qual o usuário deve aceitar novamente os termos de uso.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="fb1dc-150">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fb1dc-151">Relações</span><span class="sxs-lookup"><span data-stu-id="fb1dc-151">Relationships</span></span>
| <span data-ttu-id="fb1dc-152">Relação</span><span class="sxs-lookup"><span data-stu-id="fb1dc-152">Relationship</span></span> | <span data-ttu-id="fb1dc-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb1dc-153">Type</span></span>        | <span data-ttu-id="fb1dc-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb1dc-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb1dc-155">aceitação</span><span class="sxs-lookup"><span data-stu-id="fb1dc-155">acceptances</span></span>|<span data-ttu-id="fb1dc-156">Coleção [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="fb1dc-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="fb1dc-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-157">Read-only.</span></span> <span data-ttu-id="fb1dc-158">Informações sobre as aceitações deste contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="fb1dc-159">arquivos</span><span class="sxs-lookup"><span data-stu-id="fb1dc-159">files</span></span>|<span data-ttu-id="fb1dc-160">coleção [agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="fb1dc-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="fb1dc-161">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="fb1dc-162">**Observação:** Essa propriedade está no processo de ser preterido.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="fb1dc-163">Propriedade do **arquivo** use em vez disso.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-163">Usethe  **file** property instead.</span></span>|
|<span data-ttu-id="fb1dc-164">file</span><span class="sxs-lookup"><span data-stu-id="fb1dc-164">file</span></span>|[<span data-ttu-id="fb1dc-165">contrato de licença</span><span class="sxs-lookup"><span data-stu-id="fb1dc-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="fb1dc-166">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-166">PDFs linked to this agreement.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fb1dc-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb1dc-167">JSON representation</span></span>

<span data-ttu-id="fb1dc-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb1dc-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
