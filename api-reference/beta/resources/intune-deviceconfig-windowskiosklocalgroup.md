---
title: tipo de recurso de windowsKioskLocalGroup
description: A classe usada para identificar um grupo local para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9c5d467e70b4e2e7f60bc4898be35a2e9fefadc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964750"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="300b1-103">tipo de recurso de windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="300b1-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="300b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="300b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="300b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="300b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="300b1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="300b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="300b1-107">A classe usada para identificar um grupo local para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="300b1-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="300b1-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="300b1-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="300b1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="300b1-109">Properties</span></span>
|<span data-ttu-id="300b1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="300b1-110">Property</span></span>|<span data-ttu-id="300b1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="300b1-111">Type</span></span>|<span data-ttu-id="300b1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="300b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="300b1-113">groupName</span><span class="sxs-lookup"><span data-stu-id="300b1-113">groupName</span></span>|<span data-ttu-id="300b1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="300b1-114">String</span></span>|<span data-ttu-id="300b1-115">O nome do grupo local será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="300b1-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="300b1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="300b1-116">Relationships</span></span>
<span data-ttu-id="300b1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="300b1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="300b1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="300b1-118">JSON Representation</span></span>
<span data-ttu-id="300b1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="300b1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```





