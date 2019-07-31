---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c375b0c380cc719c8f49ba683a580133835e3a75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968159"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="34058-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="34058-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="34058-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34058-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34058-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34058-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34058-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34058-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="34058-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34058-107">Properties</span></span>
|<span data-ttu-id="34058-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34058-108">Property</span></span>|<span data-ttu-id="34058-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="34058-109">Type</span></span>|<span data-ttu-id="34058-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="34058-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34058-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34058-111">userPrincipalName</span></span>|<span data-ttu-id="34058-112">String</span><span class="sxs-lookup"><span data-stu-id="34058-112">String</span></span>|<span data-ttu-id="34058-113">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="34058-113">User name</span></span>|
|<span data-ttu-id="34058-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="34058-114">dataToSync</span></span>|<span data-ttu-id="34058-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="34058-115">Boolean</span></span>|<span data-ttu-id="34058-116">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="34058-116">Data to sync</span></span>|
|<span data-ttu-id="34058-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="34058-117">dataQuota</span></span>|<span data-ttu-id="34058-118">Int64</span><span class="sxs-lookup"><span data-stu-id="34058-118">Int64</span></span>|<span data-ttu-id="34058-119">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="34058-119">Data quota</span></span>|
|<span data-ttu-id="34058-120">dataused</span><span class="sxs-lookup"><span data-stu-id="34058-120">dataUsed</span></span>|<span data-ttu-id="34058-121">Int64</span><span class="sxs-lookup"><span data-stu-id="34058-121">Int64</span></span>|<span data-ttu-id="34058-122">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="34058-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="34058-123">Relações</span><span class="sxs-lookup"><span data-stu-id="34058-123">Relationships</span></span>
<span data-ttu-id="34058-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34058-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34058-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34058-125">JSON Representation</span></span>
<span data-ttu-id="34058-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34058-126">Here is a JSON representation of the resource.</span></span>
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





