---
title: Tipo de recurso deviceManagementConfigurationReferredSettingInformation
description: Informações de configuração referidas sobre a configuração reutilizável
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12003df5ec19bdf32b213945033eb9d5e73b9692
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868265"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a><span data-ttu-id="1f891-103">Tipo de recurso deviceManagementConfigurationReferredSettingInformation</span><span class="sxs-lookup"><span data-stu-id="1f891-103">deviceManagementConfigurationReferredSettingInformation resource type</span></span>

<span data-ttu-id="1f891-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f891-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f891-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f891-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f891-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f891-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f891-107">Informações de configuração referidas sobre a configuração reutilizável</span><span class="sxs-lookup"><span data-stu-id="1f891-107">Referred setting information about reusable setting</span></span>

## <a name="properties"></a><span data-ttu-id="1f891-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f891-108">Properties</span></span>
|<span data-ttu-id="1f891-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f891-109">Property</span></span>|<span data-ttu-id="1f891-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f891-110">Type</span></span>|<span data-ttu-id="1f891-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f891-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f891-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1f891-112">settingDefinitionId</span></span>|<span data-ttu-id="1f891-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1f891-113">String</span></span>|<span data-ttu-id="1f891-114">Definindo a id de definição que está sendo referenciada a uma configuração.</span><span class="sxs-lookup"><span data-stu-id="1f891-114">Setting definition id that is being referred to a setting.</span></span> <span data-ttu-id="1f891-115">Aplicável para a configuração reutilizável</span><span class="sxs-lookup"><span data-stu-id="1f891-115">Applicable for reusable setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f891-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1f891-116">Relationships</span></span>
<span data-ttu-id="1f891-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f891-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f891-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f891-118">JSON Representation</span></span>
<span data-ttu-id="1f891-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f891-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```




