---
title: tipo de recurso de windowsKioskAzureADGroup
description: A classe usada para identificar um grupo de AzureAD para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392567"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="d1c16-103">tipo de recurso de windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="d1c16-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="d1c16-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1c16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1c16-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1c16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1c16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d1c16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c16-107">A classe usada para identificar um grupo de AzureAD para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d1c16-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="d1c16-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="d1c16-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1c16-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1c16-109">Properties</span></span>
|<span data-ttu-id="d1c16-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1c16-110">Property</span></span>|<span data-ttu-id="d1c16-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1c16-111">Type</span></span>|<span data-ttu-id="d1c16-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1c16-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1c16-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d1c16-113">displayName</span></span>|<span data-ttu-id="d1c16-114">String</span><span class="sxs-lookup"><span data-stu-id="d1c16-114">String</span></span>|<span data-ttu-id="d1c16-115">O nome para exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d1c16-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="d1c16-116">groupId</span><span class="sxs-lookup"><span data-stu-id="d1c16-116">groupId</span></span>|<span data-ttu-id="d1c16-117">String</span><span class="sxs-lookup"><span data-stu-id="d1c16-117">String</span></span>|<span data-ttu-id="d1c16-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d1c16-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1c16-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d1c16-119">Relationships</span></span>
<span data-ttu-id="d1c16-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1c16-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1c16-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1c16-121">JSON Representation</span></span>
<span data-ttu-id="d1c16-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1c16-122">Here is a JSON representation of the resource.</span></span>
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




