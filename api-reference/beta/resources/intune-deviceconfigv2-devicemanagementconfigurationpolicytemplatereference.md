---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplateReference
description: Informações de referência do modelo de política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dee3cf25ed42f2c1ecdbf824fd807ed00c8ce91b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868300"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="42f15-103">Tipo de recurso deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="42f15-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="42f15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42f15-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42f15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42f15-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42f15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42f15-107">Informações de referência do modelo de política</span><span class="sxs-lookup"><span data-stu-id="42f15-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="42f15-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42f15-108">Properties</span></span>
|<span data-ttu-id="42f15-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42f15-109">Property</span></span>|<span data-ttu-id="42f15-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42f15-110">Type</span></span>|<span data-ttu-id="42f15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42f15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42f15-112">templateId</span><span class="sxs-lookup"><span data-stu-id="42f15-112">templateId</span></span>|<span data-ttu-id="42f15-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42f15-113">String</span></span>|<span data-ttu-id="42f15-114">ID do modelo</span><span class="sxs-lookup"><span data-stu-id="42f15-114">Template id</span></span>|
|<span data-ttu-id="42f15-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="42f15-115">templateFamily</span></span>|[<span data-ttu-id="42f15-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="42f15-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="42f15-117">Família de modelos do Modelo referenciado.</span><span class="sxs-lookup"><span data-stu-id="42f15-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="42f15-118">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42f15-118">This property is read-only.</span></span> <span data-ttu-id="42f15-119">Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="42f15-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="42f15-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="42f15-120">templateDisplayName</span></span>|<span data-ttu-id="42f15-121">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42f15-121">String</span></span>|<span data-ttu-id="42f15-122">Template Display Name of the referenced template.</span><span class="sxs-lookup"><span data-stu-id="42f15-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="42f15-123">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42f15-123">This property is read-only.</span></span>|
|<span data-ttu-id="42f15-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="42f15-124">templateDisplayVersion</span></span>|<span data-ttu-id="42f15-125">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="42f15-125">String</span></span>|<span data-ttu-id="42f15-126">Template Display Version of the referenced Template.</span><span class="sxs-lookup"><span data-stu-id="42f15-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="42f15-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42f15-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42f15-128">Relações</span><span class="sxs-lookup"><span data-stu-id="42f15-128">Relationships</span></span>
<span data-ttu-id="42f15-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42f15-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42f15-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42f15-130">JSON Representation</span></span>
<span data-ttu-id="42f15-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42f15-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```




