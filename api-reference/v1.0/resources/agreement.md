---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 045d4b9142d4bd0c4bc01392975871e0253d33c0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722556"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="c003d-103">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="c003d-103">agreement resource type</span></span>

<span data-ttu-id="c003d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c003d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c003d-105">Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c003d-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c003d-106">Você pode usar os métodos a seguir para criar e gerenciar o recurso Termos de Uso do [Azure Active Directory](/azure/active-directory/active-directory-tou) de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="c003d-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="c003d-107">Methods</span><span class="sxs-lookup"><span data-stu-id="c003d-107">Methods</span></span>

| <span data-ttu-id="c003d-108">Método</span><span class="sxs-lookup"><span data-stu-id="c003d-108">Method</span></span>       | <span data-ttu-id="c003d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c003d-109">Return Type</span></span> | <span data-ttu-id="c003d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c003d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c003d-111">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="c003d-111">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="c003d-112">[coleção agreement](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="c003d-112">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="c003d-113">Obter uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-113">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="c003d-114">Criar acordos</span><span class="sxs-lookup"><span data-stu-id="c003d-114">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="c003d-115">agreement</span><span class="sxs-lookup"><span data-stu-id="c003d-115">agreement</span></span>](agreement.md) | <span data-ttu-id="c003d-116">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="c003d-116">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="c003d-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="c003d-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="c003d-118">agreement</span><span class="sxs-lookup"><span data-stu-id="c003d-118">agreement</span></span>](agreement.md) | <span data-ttu-id="c003d-119">Ler propriedades e relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="c003d-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="c003d-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="c003d-121">agreement</span><span class="sxs-lookup"><span data-stu-id="c003d-121">agreement</span></span>](agreement.md) | <span data-ttu-id="c003d-122">Atualize um objeto agreement.</span><span class="sxs-lookup"><span data-stu-id="c003d-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="c003d-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="c003d-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="c003d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c003d-124">None</span></span> | <span data-ttu-id="c003d-125">Excluir um objeto agreement.</span><span class="sxs-lookup"><span data-stu-id="c003d-125">Delete an agreement object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c003d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c003d-126">Properties</span></span>
| <span data-ttu-id="c003d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c003d-127">Property</span></span>     | <span data-ttu-id="c003d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c003d-128">Type</span></span>        | <span data-ttu-id="c003d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c003d-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c003d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c003d-130">displayName</span></span>|<span data-ttu-id="c003d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c003d-131">String</span></span>|<span data-ttu-id="c003d-132">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-132">Display name of the agreement.</span></span> <span data-ttu-id="c003d-133">O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="c003d-134">id</span><span class="sxs-lookup"><span data-stu-id="c003d-134">id</span></span>|<span data-ttu-id="c003d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c003d-135">String</span></span>| <span data-ttu-id="c003d-136">O identificador do contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-136">The identifier of the agreement.</span></span> <span data-ttu-id="c003d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c003d-137">Read-only.</span></span>|
|<span data-ttu-id="c003d-138">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="c003d-138">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="c003d-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="c003d-139">Boolean</span></span>|<span data-ttu-id="c003d-140">Indica se os usuários finais são necessários para aceitar esse contrato em todos os dispositivos de onde eles o acessam.</span><span class="sxs-lookup"><span data-stu-id="c003d-140">Indicates whether end users are required to accept this agreement on every device that they access it from.</span></span> <span data-ttu-id="c003d-141">O usuário final deve registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso.</span><span class="sxs-lookup"><span data-stu-id="c003d-141">The end user is required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="c003d-142">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="c003d-142">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="c003d-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="c003d-143">Boolean</span></span>|<span data-ttu-id="c003d-144">Indica se o usuário precisa expandir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="c003d-144">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="c003d-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="c003d-145">termsExpiration</span></span>|[<span data-ttu-id="c003d-146">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="c003d-146">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="c003d-147">Cronograma de expiração e frequência de acordo para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="c003d-147">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="c003d-148">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="c003d-148">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="c003d-149">Duration</span><span class="sxs-lookup"><span data-stu-id="c003d-149">Duration</span></span>|<span data-ttu-id="c003d-150">A duração após a qual o usuário deve aceitar os termos de uso.</span><span class="sxs-lookup"><span data-stu-id="c003d-150">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="c003d-151">O valor é representado no formato ISO 8601 por durações.</span><span class="sxs-lookup"><span data-stu-id="c003d-151">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c003d-152">Relações</span><span class="sxs-lookup"><span data-stu-id="c003d-152">Relationships</span></span>
| <span data-ttu-id="c003d-153">Relação</span><span class="sxs-lookup"><span data-stu-id="c003d-153">Relationship</span></span> | <span data-ttu-id="c003d-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="c003d-154">Type</span></span>        | <span data-ttu-id="c003d-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="c003d-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c003d-156">acceptances</span><span class="sxs-lookup"><span data-stu-id="c003d-156">acceptances</span></span>|<span data-ttu-id="c003d-157">Coleção [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="c003d-157">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="c003d-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c003d-158">Read-only.</span></span> <span data-ttu-id="c003d-159">Informações sobre as aceitaçãos deste contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-159">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="c003d-160">arquivos</span><span class="sxs-lookup"><span data-stu-id="c003d-160">files</span></span>|<span data-ttu-id="c003d-161">[Coleção agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="c003d-161">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="c003d-162">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-162">PDFs linked to this agreement.</span></span> <span data-ttu-id="c003d-163">Essa propriedade está em processo de preterido.</span><span class="sxs-lookup"><span data-stu-id="c003d-163">This property is in the process of being deprecated.</span></span> <span data-ttu-id="c003d-164">Use a  **propriedade file** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="c003d-164">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="c003d-165">file</span><span class="sxs-lookup"><span data-stu-id="c003d-165">file</span></span>|[<span data-ttu-id="c003d-166">agreementFile</span><span class="sxs-lookup"><span data-stu-id="c003d-166">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="c003d-167">PDF padrão vinculado a este contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-167">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="c003d-168">localizações</span><span class="sxs-lookup"><span data-stu-id="c003d-168">localizations</span></span>|<span data-ttu-id="c003d-169">[Coleção agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="c003d-169">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="c003d-170">As versões localizadas dos arquivos de contrato anexados ao contrato.</span><span class="sxs-lookup"><span data-stu-id="c003d-170">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="c003d-171">versões</span><span class="sxs-lookup"><span data-stu-id="c003d-171">versions</span></span>|<span data-ttu-id="c003d-172">[Coleção agreementFileVersion](agreementfileversion.md)</span><span class="sxs-lookup"><span data-stu-id="c003d-172">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="c003d-173">O histórico de versão do arquivo de contrato localizado.</span><span class="sxs-lookup"><span data-stu-id="c003d-173">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c003d-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c003d-174">JSON representation</span></span>

<span data-ttu-id="c003d-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c003d-175">The following is a JSON representation of the resource.</span></span>

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


