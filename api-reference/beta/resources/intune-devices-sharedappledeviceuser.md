---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6142b47205640e64b8e422b1727fdf60ac8a2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524911"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="b8a4c-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="b8a4c-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="b8a4c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b8a4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8a4c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8a4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8a4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a4c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b8a4c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b8a4c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8a4c-108">Properties</span></span>
|<span data-ttu-id="b8a4c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8a4c-109">Property</span></span>|<span data-ttu-id="b8a4c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8a4c-110">Type</span></span>|<span data-ttu-id="b8a4c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8a4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a4c-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8a4c-112">userPrincipalName</span></span>|<span data-ttu-id="b8a4c-113">String</span><span class="sxs-lookup"><span data-stu-id="b8a4c-113">String</span></span>|<span data-ttu-id="b8a4c-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="b8a4c-114">User name</span></span>|
|<span data-ttu-id="b8a4c-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="b8a4c-115">dataToSync</span></span>|<span data-ttu-id="b8a4c-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8a4c-116">Boolean</span></span>|<span data-ttu-id="b8a4c-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="b8a4c-117">Data to sync</span></span>|
|<span data-ttu-id="b8a4c-118">dataquota</span><span class="sxs-lookup"><span data-stu-id="b8a4c-118">dataQuota</span></span>|<span data-ttu-id="b8a4c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b8a4c-119">Int64</span></span>|<span data-ttu-id="b8a4c-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="b8a4c-120">Data quota</span></span>|
|<span data-ttu-id="b8a4c-121">dataused</span><span class="sxs-lookup"><span data-stu-id="b8a4c-121">dataUsed</span></span>|<span data-ttu-id="b8a4c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b8a4c-122">Int64</span></span>|<span data-ttu-id="b8a4c-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="b8a4c-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8a4c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b8a4c-124">Relationships</span></span>
<span data-ttu-id="b8a4c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8a4c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8a4c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8a4c-126">JSON Representation</span></span>
<span data-ttu-id="b8a4c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8a4c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```



