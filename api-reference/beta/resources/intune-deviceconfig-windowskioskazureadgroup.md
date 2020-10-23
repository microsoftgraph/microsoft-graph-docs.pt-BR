---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 740d9b886b359eb3741034331d7b23f75b28b0c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736181"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="b21de-103">tipo de recurso windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="b21de-103">windowsKioskAzureADGroup resource type</span></span>

<span data-ttu-id="b21de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b21de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b21de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b21de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b21de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b21de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b21de-107">A classe usada para identificar um grupo do AzureAD para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="b21de-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="b21de-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="b21de-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b21de-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b21de-109">Properties</span></span>
|<span data-ttu-id="b21de-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b21de-110">Property</span></span>|<span data-ttu-id="b21de-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b21de-111">Type</span></span>|<span data-ttu-id="b21de-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b21de-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21de-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b21de-113">displayName</span></span>|<span data-ttu-id="b21de-114">String</span><span class="sxs-lookup"><span data-stu-id="b21de-114">String</span></span>|<span data-ttu-id="b21de-115">O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b21de-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="b21de-116">groupId</span><span class="sxs-lookup"><span data-stu-id="b21de-116">groupId</span></span>|<span data-ttu-id="b21de-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b21de-117">String</span></span>|<span data-ttu-id="b21de-118">A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b21de-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="b21de-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b21de-119">Relationships</span></span>
<span data-ttu-id="b21de-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b21de-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b21de-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b21de-121">JSON Representation</span></span>
<span data-ttu-id="b21de-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b21de-122">Here is a JSON representation of the resource.</span></span>
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





