---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplateReference
description: Informações de referência do modelo de política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff61ac1e881ec6bb40750d9cb43d80c6722dd79e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666496"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="6b1f5-103">Tipo de recurso deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="6b1f5-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="6b1f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b1f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b1f5-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b1f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b1f5-107">Informações de referência do modelo de política</span><span class="sxs-lookup"><span data-stu-id="6b1f5-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="6b1f5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b1f5-108">Properties</span></span>
|<span data-ttu-id="6b1f5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b1f5-109">Property</span></span>|<span data-ttu-id="6b1f5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b1f5-110">Type</span></span>|<span data-ttu-id="6b1f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b1f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b1f5-112">templateId</span><span class="sxs-lookup"><span data-stu-id="6b1f5-112">templateId</span></span>|<span data-ttu-id="6b1f5-113">String</span><span class="sxs-lookup"><span data-stu-id="6b1f5-113">String</span></span>|<span data-ttu-id="6b1f5-114">ID do modelo</span><span class="sxs-lookup"><span data-stu-id="6b1f5-114">Template id</span></span>|
|<span data-ttu-id="6b1f5-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="6b1f5-115">templateFamily</span></span>|[<span data-ttu-id="6b1f5-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="6b1f5-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="6b1f5-117">Família de modelos do Modelo referenciado.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="6b1f5-118">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-118">This property is read-only.</span></span> <span data-ttu-id="6b1f5-119">Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="6b1f5-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="6b1f5-120">templateDisplayName</span></span>|<span data-ttu-id="6b1f5-121">String</span><span class="sxs-lookup"><span data-stu-id="6b1f5-121">String</span></span>|<span data-ttu-id="6b1f5-122">Template Display Name of the referenced template.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="6b1f5-123">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-123">This property is read-only.</span></span>|
|<span data-ttu-id="6b1f5-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="6b1f5-124">templateDisplayVersion</span></span>|<span data-ttu-id="6b1f5-125">String</span><span class="sxs-lookup"><span data-stu-id="6b1f5-125">String</span></span>|<span data-ttu-id="6b1f5-126">Template Display Version of the referenced Template.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="6b1f5-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b1f5-128">Relações</span><span class="sxs-lookup"><span data-stu-id="6b1f5-128">Relationships</span></span>
<span data-ttu-id="6b1f5-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6b1f5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b1f5-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b1f5-130">JSON Representation</span></span>
<span data-ttu-id="6b1f5-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b1f5-131">Here is a JSON representation of the resource.</span></span>
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




