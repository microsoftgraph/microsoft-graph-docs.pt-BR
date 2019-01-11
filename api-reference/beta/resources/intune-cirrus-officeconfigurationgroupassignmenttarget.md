---
title: tipo de recurso de officeConfigurationGroupAssignmentTarget
description: Configuração de cliente do Office AAD destino de atribuição de grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2fe6a668c1f490c167fe61496af14cf2654cebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814767"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="c702a-103">tipo de recurso de officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c702a-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c702a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c702a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c702a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c702a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c702a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c702a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c702a-107">Configuração de cliente do Office AAD destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="c702a-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="c702a-108">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c702a-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c702a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c702a-109">Properties</span></span>
|<span data-ttu-id="c702a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c702a-110">Property</span></span>|<span data-ttu-id="c702a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c702a-111">Type</span></span>|<span data-ttu-id="c702a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c702a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c702a-113">groupId</span><span class="sxs-lookup"><span data-stu-id="c702a-113">groupId</span></span>|<span data-ttu-id="c702a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c702a-114">String</span></span>|<span data-ttu-id="c702a-115">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c702a-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c702a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c702a-116">Relationships</span></span>
<span data-ttu-id="c702a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c702a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c702a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c702a-118">JSON Representation</span></span>
<span data-ttu-id="c702a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c702a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



