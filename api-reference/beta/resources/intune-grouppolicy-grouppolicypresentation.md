---
title: tipo de recurso de groupPolicyPresentation
description: A entidade base para a apresentação de exibição de qualquer uma das opções adicionais em uma definição de diretiva de grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429247"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="9e58f-103">tipo de recurso de groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9e58f-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="9e58f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e58f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e58f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e58f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e58f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9e58f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e58f-107">A entidade base para a apresentação de exibição de qualquer uma das opções adicionais em uma definição de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="9e58f-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="9e58f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e58f-108">Methods</span></span>
|<span data-ttu-id="9e58f-109">Método</span><span class="sxs-lookup"><span data-stu-id="9e58f-109">Method</span></span>|<span data-ttu-id="9e58f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e58f-110">Return Type</span></span>|<span data-ttu-id="9e58f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e58f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e58f-112">Obter groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9e58f-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="9e58f-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9e58f-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9e58f-114">Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="9e58f-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="9e58f-115">Atualizar groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9e58f-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="9e58f-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="9e58f-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="9e58f-117">Atualize as propriedades de um objeto [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="9e58f-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e58f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e58f-118">Properties</span></span>
|<span data-ttu-id="9e58f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e58f-119">Property</span></span>|<span data-ttu-id="9e58f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e58f-120">Type</span></span>|<span data-ttu-id="9e58f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e58f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e58f-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="9e58f-122">label</span></span>|<span data-ttu-id="9e58f-123">String</span><span class="sxs-lookup"><span data-stu-id="9e58f-123">String</span></span>|<span data-ttu-id="9e58f-124">Rótulo de texto localizado para qualquer entidade de apresentação.</span><span class="sxs-lookup"><span data-stu-id="9e58f-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9e58f-125">O valor padrão é vazio.</span><span class="sxs-lookup"><span data-stu-id="9e58f-125">The default value is empty.</span></span>|
|<span data-ttu-id="9e58f-126">id</span><span class="sxs-lookup"><span data-stu-id="9e58f-126">id</span></span>|<span data-ttu-id="9e58f-127">String</span><span class="sxs-lookup"><span data-stu-id="9e58f-127">String</span></span>|<span data-ttu-id="9e58f-128">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e58f-128">Key of the entity.</span></span>|
|<span data-ttu-id="9e58f-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e58f-129">lastModifiedDateTime</span></span>|<span data-ttu-id="9e58f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e58f-130">DateTimeOffset</span></span>|<span data-ttu-id="9e58f-131">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9e58f-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e58f-132">Relações</span><span class="sxs-lookup"><span data-stu-id="9e58f-132">Relationships</span></span>
|<span data-ttu-id="9e58f-133">Relação</span><span class="sxs-lookup"><span data-stu-id="9e58f-133">Relationship</span></span>|<span data-ttu-id="9e58f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e58f-134">Type</span></span>|<span data-ttu-id="9e58f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e58f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e58f-136">definição</span><span class="sxs-lookup"><span data-stu-id="9e58f-136">definition</span></span>|[<span data-ttu-id="9e58f-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9e58f-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="9e58f-138">A definição de política de grupo associada à apresentação.</span><span class="sxs-lookup"><span data-stu-id="9e58f-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e58f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e58f-139">JSON Representation</span></span>
<span data-ttu-id="9e58f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e58f-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




