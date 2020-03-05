---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6569dc23786b9587ab7290859ff9a151a3e370c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525506"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="b8ffa-103">tipo de recurso windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="b8ffa-103">windowsKioskAzureADGroup resource type</span></span>

<span data-ttu-id="b8ffa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b8ffa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8ffa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8ffa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8ffa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8ffa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ffa-107">A classe usada para identificar um grupo do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="b8ffa-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="b8ffa-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="b8ffa-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8ffa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8ffa-109">Properties</span></span>
|<span data-ttu-id="b8ffa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8ffa-110">Property</span></span>|<span data-ttu-id="b8ffa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8ffa-111">Type</span></span>|<span data-ttu-id="b8ffa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8ffa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ffa-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b8ffa-113">displayName</span></span>|<span data-ttu-id="b8ffa-114">String</span><span class="sxs-lookup"><span data-stu-id="b8ffa-114">String</span></span>|<span data-ttu-id="b8ffa-115">O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b8ffa-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="b8ffa-116">groupId</span><span class="sxs-lookup"><span data-stu-id="b8ffa-116">groupId</span></span>|<span data-ttu-id="b8ffa-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8ffa-117">String</span></span>|<span data-ttu-id="b8ffa-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b8ffa-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ffa-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b8ffa-119">Relationships</span></span>
<span data-ttu-id="b8ffa-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8ffa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8ffa-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8ffa-121">JSON Representation</span></span>
<span data-ttu-id="b8ffa-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8ffa-122">Here is a JSON representation of the resource.</span></span>
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



