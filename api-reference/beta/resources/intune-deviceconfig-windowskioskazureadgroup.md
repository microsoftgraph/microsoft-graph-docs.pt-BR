---
title: tipo de recurso de windowsKioskAzureADGroup
description: A classe usada para identificar um grupo de AzureAD para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16c2b17220a92f9f230b786238b1195e2af48d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849865"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="35ae0-103">tipo de recurso de windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="35ae0-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="35ae0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35ae0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35ae0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35ae0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35ae0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35ae0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35ae0-107">A classe usada para identificar um grupo de AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="35ae0-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="35ae0-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="35ae0-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35ae0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35ae0-109">Properties</span></span>
|<span data-ttu-id="35ae0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35ae0-110">Property</span></span>|<span data-ttu-id="35ae0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="35ae0-111">Type</span></span>|<span data-ttu-id="35ae0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="35ae0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35ae0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="35ae0-113">displayName</span></span>|<span data-ttu-id="35ae0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35ae0-114">String</span></span>|<span data-ttu-id="35ae0-115">O nome para exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="35ae0-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="35ae0-116">groupId</span><span class="sxs-lookup"><span data-stu-id="35ae0-116">groupId</span></span>|<span data-ttu-id="35ae0-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35ae0-117">String</span></span>|<span data-ttu-id="35ae0-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="35ae0-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="35ae0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="35ae0-119">Relationships</span></span>
<span data-ttu-id="35ae0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35ae0-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35ae0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35ae0-121">JSON Representation</span></span>
<span data-ttu-id="35ae0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35ae0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





