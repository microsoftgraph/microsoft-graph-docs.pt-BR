---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff51ad89600919fb1ed2c3bb506a53178ccdc445
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941748"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="34311-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="34311-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="34311-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34311-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34311-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34311-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34311-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="34311-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="34311-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34311-107">Properties</span></span>
|<span data-ttu-id="34311-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34311-108">Property</span></span>|<span data-ttu-id="34311-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="34311-109">Type</span></span>|<span data-ttu-id="34311-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="34311-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34311-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34311-111">userPrincipalName</span></span>|<span data-ttu-id="34311-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34311-112">String</span></span>|<span data-ttu-id="34311-113">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="34311-113">User name</span></span>|
|<span data-ttu-id="34311-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="34311-114">dataToSync</span></span>|<span data-ttu-id="34311-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="34311-115">Boolean</span></span>|<span data-ttu-id="34311-116">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="34311-116">Data to sync</span></span>|
|<span data-ttu-id="34311-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="34311-117">dataQuota</span></span>|<span data-ttu-id="34311-118">Int64</span><span class="sxs-lookup"><span data-stu-id="34311-118">Int64</span></span>|<span data-ttu-id="34311-119">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="34311-119">Data quota</span></span>|
|<span data-ttu-id="34311-120">dataused</span><span class="sxs-lookup"><span data-stu-id="34311-120">dataUsed</span></span>|<span data-ttu-id="34311-121">Int64</span><span class="sxs-lookup"><span data-stu-id="34311-121">Int64</span></span>|<span data-ttu-id="34311-122">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="34311-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="34311-123">Relações</span><span class="sxs-lookup"><span data-stu-id="34311-123">Relationships</span></span>
<span data-ttu-id="34311-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34311-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34311-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34311-125">JSON Representation</span></span>
<span data-ttu-id="34311-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34311-126">Here is a JSON representation of the resource.</span></span>
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




