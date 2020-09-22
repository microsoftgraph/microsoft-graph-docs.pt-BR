---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: a6b987e36769102ee32eeb9509554f8e78fed9d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067501"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="ac52d-103">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-103">agreement resource type</span></span>

<span data-ttu-id="ac52d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac52d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac52d-105">Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ac52d-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ac52d-106">Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="ac52d-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="ac52d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac52d-107">Methods</span></span>

| <span data-ttu-id="ac52d-108">Método</span><span class="sxs-lookup"><span data-stu-id="ac52d-108">Method</span></span>       | <span data-ttu-id="ac52d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac52d-109">Return Type</span></span> | <span data-ttu-id="ac52d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac52d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ac52d-111">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="ac52d-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="ac52d-112">contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-112">agreement</span></span>](agreement.md) | <span data-ttu-id="ac52d-113">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="ac52d-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="ac52d-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="ac52d-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="ac52d-115">coleção de [contratos](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="ac52d-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="ac52d-116">Obtenha uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="ac52d-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="ac52d-118">contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-118">agreement</span></span>](agreement.md) | <span data-ttu-id="ac52d-119">Leia as propriedades e as relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="ac52d-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="ac52d-121">contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-121">agreement</span></span>](agreement.md) | <span data-ttu-id="ac52d-122">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="ac52d-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="ac52d-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="ac52d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac52d-124">None</span></span> | <span data-ttu-id="ac52d-125">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="ac52d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac52d-126">Properties</span></span>
| <span data-ttu-id="ac52d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac52d-127">Property</span></span>     | <span data-ttu-id="ac52d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac52d-128">Type</span></span>        | <span data-ttu-id="ac52d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac52d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac52d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ac52d-130">displayName</span></span>|<span data-ttu-id="ac52d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac52d-131">String</span></span>|<span data-ttu-id="ac52d-132">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-132">Display name of the agreement.</span></span> <span data-ttu-id="ac52d-133">O nome para exibição é usado para o controle interno do contrato, mas não é exibido para os usuários finais que exibem o contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="ac52d-134">id</span><span class="sxs-lookup"><span data-stu-id="ac52d-134">id</span></span>|<span data-ttu-id="ac52d-135">String</span><span class="sxs-lookup"><span data-stu-id="ac52d-135">String</span></span>| <span data-ttu-id="ac52d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac52d-136">Read-only.</span></span>|
|<span data-ttu-id="ac52d-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="ac52d-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="ac52d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac52d-138">Boolean</span></span>|<span data-ttu-id="ac52d-139">Essa configuração permite que você exija que os usuários finais aceitem este contrato em todos os dispositivos dos quais eles estão acessando-os.</span><span class="sxs-lookup"><span data-stu-id="ac52d-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="ac52d-140">O usuário final será solicitado a registrar o dispositivo no Azure AD, caso ainda não tenha feito isso.</span><span class="sxs-lookup"><span data-stu-id="ac52d-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="ac52d-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="ac52d-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="ac52d-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac52d-142">Boolean</span></span>|<span data-ttu-id="ac52d-143">Indica se o usuário tem que expandir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="ac52d-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="ac52d-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="ac52d-144">termsExpiration</span></span>|[<span data-ttu-id="ac52d-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="ac52d-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="ac52d-146">Cronograma de expiração e frequência de contrato para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="ac52d-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="ac52d-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="ac52d-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="ac52d-148">Duração</span><span class="sxs-lookup"><span data-stu-id="ac52d-148">Duration</span></span>|<span data-ttu-id="ac52d-149">A duração após a qual o usuário deve aceitar novamente os termos de uso.</span><span class="sxs-lookup"><span data-stu-id="ac52d-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="ac52d-150">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="ac52d-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="ac52d-151">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ac52d-151">Relationships</span></span>
| <span data-ttu-id="ac52d-152">Relação</span><span class="sxs-lookup"><span data-stu-id="ac52d-152">Relationship</span></span> | <span data-ttu-id="ac52d-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac52d-153">Type</span></span>        | <span data-ttu-id="ac52d-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac52d-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac52d-155">aceitação</span><span class="sxs-lookup"><span data-stu-id="ac52d-155">acceptances</span></span>|<span data-ttu-id="ac52d-156">Coleção [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="ac52d-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="ac52d-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac52d-157">Read-only.</span></span> <span data-ttu-id="ac52d-158">Informações sobre as aceitações deste contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="ac52d-159">arquivos</span><span class="sxs-lookup"><span data-stu-id="ac52d-159">files</span></span>|<span data-ttu-id="ac52d-160">coleção [agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="ac52d-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="ac52d-161">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="ac52d-162">**Observação:** Essa propriedade está no processo de ser preterido.</span><span class="sxs-lookup"><span data-stu-id="ac52d-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="ac52d-163">Propriedade do  **arquivo** use em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ac52d-163">Usethe  **file** property instead.</span></span>|
|<span data-ttu-id="ac52d-164">file</span><span class="sxs-lookup"><span data-stu-id="ac52d-164">file</span></span>|[<span data-ttu-id="ac52d-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="ac52d-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="ac52d-166">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="ac52d-166">PDFs linked to this agreement.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ac52d-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac52d-167">JSON representation</span></span>

<span data-ttu-id="ac52d-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac52d-168">The following is a JSON representation of the resource.</span></span>

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


