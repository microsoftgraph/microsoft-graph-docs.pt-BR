---
title: tipo de recurso de officeConfigurationGroupAssignmentTarget
description: Configuração de cliente do Office AAD destino de atribuição de grupo.
ms.openlocfilehash: 263e48bfc5800231a9f36159e802f65294e6ac02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038990"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="406db-103">tipo de recurso de officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="406db-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="406db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="406db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="406db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="406db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="406db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="406db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="406db-107">Configuração de cliente do Office AAD destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="406db-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="406db-108">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="406db-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="406db-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="406db-109">Properties</span></span>
|<span data-ttu-id="406db-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="406db-110">Property</span></span>|<span data-ttu-id="406db-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="406db-111">Type</span></span>|<span data-ttu-id="406db-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="406db-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="406db-113">groupId</span><span class="sxs-lookup"><span data-stu-id="406db-113">groupId</span></span>|<span data-ttu-id="406db-114">String</span><span class="sxs-lookup"><span data-stu-id="406db-114">String</span></span>|<span data-ttu-id="406db-115">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="406db-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="406db-116">Relações</span><span class="sxs-lookup"><span data-stu-id="406db-116">Relationships</span></span>
<span data-ttu-id="406db-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="406db-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="406db-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="406db-118">JSON Representation</span></span>
<span data-ttu-id="406db-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="406db-119">Here is a JSON representation of the resource.</span></span>
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



