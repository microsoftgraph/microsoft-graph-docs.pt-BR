---
title: tipo de recurso de windowsKioskAzureADGroup
description: A classe usada para identificar um grupo de AzureAD para a configuração de quiosque
ms.openlocfilehash: 4853013c9c1e9d4c276ee5e2ba83cb8b36afd06c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033614"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="fbb85-103">tipo de recurso de windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="fbb85-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="fbb85-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbb85-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbb85-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbb85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbb85-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fbb85-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbb85-107">A classe usada para identificar um grupo de AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="fbb85-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="fbb85-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="fbb85-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbb85-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbb85-109">Properties</span></span>
|<span data-ttu-id="fbb85-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbb85-110">Property</span></span>|<span data-ttu-id="fbb85-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbb85-111">Type</span></span>|<span data-ttu-id="fbb85-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb85-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb85-113">displayName</span><span class="sxs-lookup"><span data-stu-id="fbb85-113">displayName</span></span>|<span data-ttu-id="fbb85-114">String</span><span class="sxs-lookup"><span data-stu-id="fbb85-114">String</span></span>|<span data-ttu-id="fbb85-115">O nome para exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="fbb85-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="fbb85-116">groupId</span><span class="sxs-lookup"><span data-stu-id="fbb85-116">groupId</span></span>|<span data-ttu-id="fbb85-117">String</span><span class="sxs-lookup"><span data-stu-id="fbb85-117">String</span></span>|<span data-ttu-id="fbb85-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="fbb85-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbb85-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fbb85-119">Relationships</span></span>
<span data-ttu-id="fbb85-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbb85-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbb85-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbb85-121">JSON Representation</span></span>
<span data-ttu-id="fbb85-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbb85-122">Here is a JSON representation of the resource.</span></span>
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





