---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: bb1de9d03de4d891ef91d076ccbd41e6b569e3f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433198"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="4f32c-103">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="4f32c-103">agreement resource type</span></span>

<span data-ttu-id="4f32c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f32c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f32c-105">Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4f32c-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="4f32c-106">Você pode usar os métodos a seguir para criar e gerenciar o recurso Termos de Uso do [Azure Active Directory](/azure/active-directory/active-directory-tou) de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="4f32c-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="4f32c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="4f32c-107">Methods</span></span>

| <span data-ttu-id="4f32c-108">Método</span><span class="sxs-lookup"><span data-stu-id="4f32c-108">Method</span></span>       | <span data-ttu-id="4f32c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4f32c-109">Return Type</span></span> | <span data-ttu-id="4f32c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f32c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4f32c-111">Criar acordos</span><span class="sxs-lookup"><span data-stu-id="4f32c-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="4f32c-112">agreement</span><span class="sxs-lookup"><span data-stu-id="4f32c-112">agreement</span></span>](agreement.md) | <span data-ttu-id="4f32c-113">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="4f32c-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="4f32c-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="4f32c-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="4f32c-115">[coleção agreement](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="4f32c-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="4f32c-116">Obter uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="4f32c-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="4f32c-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="4f32c-118">agreement</span><span class="sxs-lookup"><span data-stu-id="4f32c-118">agreement</span></span>](agreement.md) | <span data-ttu-id="4f32c-119">Ler propriedades e relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="4f32c-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="4f32c-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="4f32c-121">agreement</span><span class="sxs-lookup"><span data-stu-id="4f32c-121">agreement</span></span>](agreement.md) | <span data-ttu-id="4f32c-122">Atualize um objeto agreement.</span><span class="sxs-lookup"><span data-stu-id="4f32c-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="4f32c-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="4f32c-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="4f32c-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="4f32c-124">None</span></span> | <span data-ttu-id="4f32c-125">Excluir um objeto agreement.</span><span class="sxs-lookup"><span data-stu-id="4f32c-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="4f32c-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f32c-126">Properties</span></span>
| <span data-ttu-id="4f32c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f32c-127">Property</span></span>     | <span data-ttu-id="4f32c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f32c-128">Type</span></span>        | <span data-ttu-id="4f32c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f32c-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f32c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4f32c-130">displayName</span></span>|<span data-ttu-id="4f32c-131">String</span><span class="sxs-lookup"><span data-stu-id="4f32c-131">String</span></span>|<span data-ttu-id="4f32c-132">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-132">Display name of the agreement.</span></span> <span data-ttu-id="4f32c-133">O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="4f32c-134">id</span><span class="sxs-lookup"><span data-stu-id="4f32c-134">id</span></span>|<span data-ttu-id="4f32c-135">String</span><span class="sxs-lookup"><span data-stu-id="4f32c-135">String</span></span>| <span data-ttu-id="4f32c-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f32c-136">Read-only.</span></span>|
|<span data-ttu-id="4f32c-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="4f32c-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="4f32c-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="4f32c-138">Boolean</span></span>|<span data-ttu-id="4f32c-139">Essa configuração permite exigir que os usuários finais aceitem esse contrato em todos os dispositivos de onde eles estão acessando.</span><span class="sxs-lookup"><span data-stu-id="4f32c-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="4f32c-140">O usuário final será necessário para registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso.</span><span class="sxs-lookup"><span data-stu-id="4f32c-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="4f32c-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="4f32c-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="4f32c-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="4f32c-142">Boolean</span></span>|<span data-ttu-id="4f32c-143">Indica se o usuário precisa expandir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="4f32c-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="4f32c-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="4f32c-144">termsExpiration</span></span>|[<span data-ttu-id="4f32c-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="4f32c-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="4f32c-146">Cronograma de expiração e frequência de acordo para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="4f32c-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="4f32c-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="4f32c-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="4f32c-148">Duração</span><span class="sxs-lookup"><span data-stu-id="4f32c-148">Duration</span></span>|<span data-ttu-id="4f32c-149">A duração após a qual o usuário deve aceitar os termos de uso.</span><span class="sxs-lookup"><span data-stu-id="4f32c-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="4f32c-150">O valor é representado no formato ISO 8601 por durações.</span><span class="sxs-lookup"><span data-stu-id="4f32c-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4f32c-151">Relações</span><span class="sxs-lookup"><span data-stu-id="4f32c-151">Relationships</span></span>
| <span data-ttu-id="4f32c-152">Relação</span><span class="sxs-lookup"><span data-stu-id="4f32c-152">Relationship</span></span> | <span data-ttu-id="4f32c-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f32c-153">Type</span></span>        | <span data-ttu-id="4f32c-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f32c-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f32c-155">acceptances</span><span class="sxs-lookup"><span data-stu-id="4f32c-155">acceptances</span></span>|<span data-ttu-id="4f32c-156">Coleção [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="4f32c-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="4f32c-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f32c-157">Read-only.</span></span> <span data-ttu-id="4f32c-158">Informações sobre as aceitaçãos deste contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="4f32c-159">arquivos</span><span class="sxs-lookup"><span data-stu-id="4f32c-159">files</span></span>|<span data-ttu-id="4f32c-160">[Coleção agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="4f32c-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="4f32c-161">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="4f32c-162">**Observação:** Essa propriedade está em processo de preterido.</span><span class="sxs-lookup"><span data-stu-id="4f32c-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="4f32c-163">Use a  **propriedade file** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="4f32c-163">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="4f32c-164">file</span><span class="sxs-lookup"><span data-stu-id="4f32c-164">file</span></span>|[<span data-ttu-id="4f32c-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="4f32c-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="4f32c-166">PDF padrão vinculado a este contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-166">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="4f32c-167">file/localizações</span><span class="sxs-lookup"><span data-stu-id="4f32c-167">file/localizations</span></span>|<span data-ttu-id="4f32c-168">[Coleção agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="4f32c-168">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="4f32c-169">As versões localizadas dos arquivos de contrato anexados ao contrato.</span><span class="sxs-lookup"><span data-stu-id="4f32c-169">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="4f32c-170">file/localizations/{localizationId}/versions</span><span class="sxs-lookup"><span data-stu-id="4f32c-170">file/localizations/{localizationId}/versions</span></span>|<span data-ttu-id="4f32c-171">[Coleção agreementFileVersion](agreementfileversion.md)</span><span class="sxs-lookup"><span data-stu-id="4f32c-171">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="4f32c-172">O histórico de versão do arquivo de contrato localizado.</span><span class="sxs-lookup"><span data-stu-id="4f32c-172">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4f32c-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f32c-173">JSON representation</span></span>

<span data-ttu-id="4f32c-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f32c-174">The following is a JSON representation of the resource.</span></span>

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


