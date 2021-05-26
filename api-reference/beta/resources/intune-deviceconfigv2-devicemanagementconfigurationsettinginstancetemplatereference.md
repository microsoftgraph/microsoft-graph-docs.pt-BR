---
title: Tipo de recurso deviceManagementConfigurationSettingInstanceTemplateReference
description: Definindo informações de referência do modelo de instância
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d537791337f13ba9fcf3bd19ef77b1c0aec58463
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666771"
---
# <a name="devicemanagementconfigurationsettinginstancetemplatereference-resource-type"></a><span data-ttu-id="c8a1c-103">Tipo de recurso deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="c8a1c-103">deviceManagementConfigurationSettingInstanceTemplateReference resource type</span></span>

<span data-ttu-id="c8a1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8a1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8a1c-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8a1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8a1c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8a1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8a1c-107">Definindo informações de referência do modelo de instância</span><span class="sxs-lookup"><span data-stu-id="c8a1c-107">Setting instance template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="c8a1c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8a1c-108">Properties</span></span>
|<span data-ttu-id="c8a1c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8a1c-109">Property</span></span>|<span data-ttu-id="c8a1c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8a1c-110">Type</span></span>|<span data-ttu-id="c8a1c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8a1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a1c-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="c8a1c-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="c8a1c-113">String</span><span class="sxs-lookup"><span data-stu-id="c8a1c-113">String</span></span>|<span data-ttu-id="c8a1c-114">ID do modelo de instância de configuração</span><span class="sxs-lookup"><span data-stu-id="c8a1c-114">Setting instance template id</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8a1c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c8a1c-115">Relationships</span></span>
<span data-ttu-id="c8a1c-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c8a1c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8a1c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8a1c-117">JSON Representation</span></span>
<span data-ttu-id="c8a1c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8a1c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
  "settingInstanceTemplateId": "String"
}
```




