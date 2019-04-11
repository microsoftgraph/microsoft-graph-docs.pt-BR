---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3224f55f4a5158fb8c0850a4dbea7e6bcf8d18d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778051"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="d2262-103">tipo de recurso windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="d2262-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="d2262-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2262-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2262-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2262-106">A classe usada para identificar um grupo do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="d2262-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="d2262-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="d2262-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2262-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2262-108">Properties</span></span>
|<span data-ttu-id="d2262-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2262-109">Property</span></span>|<span data-ttu-id="d2262-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2262-110">Type</span></span>|<span data-ttu-id="d2262-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2262-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2262-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d2262-112">displayName</span></span>|<span data-ttu-id="d2262-113">String</span><span class="sxs-lookup"><span data-stu-id="d2262-113">String</span></span>|<span data-ttu-id="d2262-114">O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d2262-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="d2262-115">groupId</span><span class="sxs-lookup"><span data-stu-id="d2262-115">groupId</span></span>|<span data-ttu-id="d2262-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2262-116">String</span></span>|<span data-ttu-id="d2262-117">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="d2262-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2262-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d2262-118">Relationships</span></span>
<span data-ttu-id="d2262-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d2262-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2262-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2262-120">JSON Representation</span></span>
<span data-ttu-id="d2262-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2262-121">Here is a JSON representation of the resource.</span></span>
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





