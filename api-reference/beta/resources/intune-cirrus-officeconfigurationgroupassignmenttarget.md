---
title: tipo de recurso de officeConfigurationGroupAssignmentTarget
description: Configuração de cliente do Office AAD destino de atribuição de grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422744"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="00941-103">tipo de recurso de officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="00941-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="00941-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="00941-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00941-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00941-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00941-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="00941-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00941-107">Configuração de cliente do Office AAD destino de atribuição de grupo.</span><span class="sxs-lookup"><span data-stu-id="00941-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="00941-108">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="00941-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00941-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00941-109">Properties</span></span>
|<span data-ttu-id="00941-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00941-110">Property</span></span>|<span data-ttu-id="00941-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="00941-111">Type</span></span>|<span data-ttu-id="00941-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="00941-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00941-113">groupId</span><span class="sxs-lookup"><span data-stu-id="00941-113">groupId</span></span>|<span data-ttu-id="00941-114">String</span><span class="sxs-lookup"><span data-stu-id="00941-114">String</span></span>|<span data-ttu-id="00941-115">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00941-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00941-116">Relações</span><span class="sxs-lookup"><span data-stu-id="00941-116">Relationships</span></span>
<span data-ttu-id="00941-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00941-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00941-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00941-118">JSON Representation</span></span>
<span data-ttu-id="00941-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00941-119">Here is a JSON representation of the resource.</span></span>
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



