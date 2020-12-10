---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: af4a6079aaed846af3322a94eb961315f7291686
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617098"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="4a401-103">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-103">agreement resource type</span></span>

<span data-ttu-id="4a401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a401-105">Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4a401-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="4a401-106">Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="4a401-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="4a401-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a401-107">Methods</span></span>

| <span data-ttu-id="4a401-108">Método</span><span class="sxs-lookup"><span data-stu-id="4a401-108">Method</span></span>       | <span data-ttu-id="4a401-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a401-109">Return Type</span></span> | <span data-ttu-id="4a401-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a401-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4a401-111">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="4a401-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="4a401-112">contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-112">agreement</span></span>](agreement.md) | <span data-ttu-id="4a401-113">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="4a401-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="4a401-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="4a401-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="4a401-115">coleção de [contratos](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="4a401-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="4a401-116">Obtenha uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="4a401-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="4a401-118">contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-118">agreement</span></span>](agreement.md) | <span data-ttu-id="4a401-119">Leia as propriedades e as relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="4a401-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="4a401-121">contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-121">agreement</span></span>](agreement.md) | <span data-ttu-id="4a401-122">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="4a401-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="4a401-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="4a401-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a401-124">None</span></span> | <span data-ttu-id="4a401-125">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="4a401-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a401-126">Properties</span></span>
| <span data-ttu-id="4a401-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a401-127">Property</span></span>     | <span data-ttu-id="4a401-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a401-128">Type</span></span>        | <span data-ttu-id="4a401-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a401-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a401-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4a401-130">displayName</span></span>|<span data-ttu-id="4a401-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a401-131">String</span></span>|<span data-ttu-id="4a401-132">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-132">Display name of the agreement.</span></span> <span data-ttu-id="4a401-133">O nome para exibição é usado para o controle interno do contrato, mas não é exibido para os usuários finais que exibem o contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="4a401-134">id</span><span class="sxs-lookup"><span data-stu-id="4a401-134">id</span></span>|<span data-ttu-id="4a401-135">String</span><span class="sxs-lookup"><span data-stu-id="4a401-135">String</span></span>| <span data-ttu-id="4a401-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a401-136">Read-only.</span></span>|
|<span data-ttu-id="4a401-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="4a401-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="4a401-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a401-138">Boolean</span></span>|<span data-ttu-id="4a401-139">Essa configuração permite que você exija que os usuários finais aceitem este contrato em todos os dispositivos dos quais eles estão acessando-os.</span><span class="sxs-lookup"><span data-stu-id="4a401-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="4a401-140">O usuário final será solicitado a registrar o dispositivo no Azure AD, caso ainda não tenha feito isso.</span><span class="sxs-lookup"><span data-stu-id="4a401-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="4a401-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="4a401-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="4a401-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a401-142">Boolean</span></span>|<span data-ttu-id="4a401-143">Indica se o usuário tem que expandir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="4a401-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="4a401-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="4a401-144">termsExpiration</span></span>|[<span data-ttu-id="4a401-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="4a401-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="4a401-146">Cronograma de expiração e frequência de contrato para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="4a401-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="4a401-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="4a401-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="4a401-148">Duração</span><span class="sxs-lookup"><span data-stu-id="4a401-148">Duration</span></span>|<span data-ttu-id="4a401-149">A duração após a qual o usuário deve aceitar novamente os termos de uso.</span><span class="sxs-lookup"><span data-stu-id="4a401-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="4a401-150">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="4a401-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4a401-151">Relações</span><span class="sxs-lookup"><span data-stu-id="4a401-151">Relationships</span></span>
| <span data-ttu-id="4a401-152">Relação</span><span class="sxs-lookup"><span data-stu-id="4a401-152">Relationship</span></span> | <span data-ttu-id="4a401-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a401-153">Type</span></span>        | <span data-ttu-id="4a401-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a401-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a401-155">aceitação</span><span class="sxs-lookup"><span data-stu-id="4a401-155">acceptances</span></span>|<span data-ttu-id="4a401-156">Coleção [agreementAcceptance](agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="4a401-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="4a401-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a401-157">Read-only.</span></span> <span data-ttu-id="4a401-158">Informações sobre as aceitações deste contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="4a401-159">arquivos</span><span class="sxs-lookup"><span data-stu-id="4a401-159">files</span></span>|<span data-ttu-id="4a401-160">coleção [agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="4a401-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="4a401-161">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="4a401-162">**Observação:** Essa propriedade está no processo de ser preterido.</span><span class="sxs-lookup"><span data-stu-id="4a401-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="4a401-163">Em vez disso, use a propriedade  **File** .</span><span class="sxs-lookup"><span data-stu-id="4a401-163">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="4a401-164">file</span><span class="sxs-lookup"><span data-stu-id="4a401-164">file</span></span>|[<span data-ttu-id="4a401-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="4a401-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="4a401-166">PDF padrão vinculado a este contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-166">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="4a401-167">arquivos/localizações</span><span class="sxs-lookup"><span data-stu-id="4a401-167">file/localizations</span></span>|<span data-ttu-id="4a401-168">coleção [agreementFileLocalization](agreementfilelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="4a401-168">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="4a401-169">As versões localizadas dos arquivos de contrato anexados ao contrato.</span><span class="sxs-lookup"><span data-stu-id="4a401-169">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="4a401-170">arquivo/localizações/{localizações}/versões</span><span class="sxs-lookup"><span data-stu-id="4a401-170">file/localizations/{localizationId}/versions</span></span>|<span data-ttu-id="4a401-171">coleção [agreementFileVersion](agreementfileversion.md)</span><span class="sxs-lookup"><span data-stu-id="4a401-171">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="4a401-172">O histórico de versão do arquivo de contrato localizado.</span><span class="sxs-lookup"><span data-stu-id="4a401-172">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4a401-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a401-173">JSON representation</span></span>

<span data-ttu-id="4a401-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a401-174">The following is a JSON representation of the resource.</span></span>

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


