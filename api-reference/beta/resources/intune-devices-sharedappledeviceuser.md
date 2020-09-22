---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df9f47aa4655c0e360d5c89f38443f5f8dc499ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081003"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="b1205-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="b1205-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="b1205-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1205-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1205-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1205-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1205-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1205-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1205-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1205-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b1205-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1205-108">Properties</span></span>
|<span data-ttu-id="b1205-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1205-109">Property</span></span>|<span data-ttu-id="b1205-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1205-110">Type</span></span>|<span data-ttu-id="b1205-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1205-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1205-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1205-112">userPrincipalName</span></span>|<span data-ttu-id="b1205-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1205-113">String</span></span>|<span data-ttu-id="b1205-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="b1205-114">User name</span></span>|
|<span data-ttu-id="b1205-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="b1205-115">dataToSync</span></span>|<span data-ttu-id="b1205-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1205-116">Boolean</span></span>|<span data-ttu-id="b1205-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="b1205-117">Data to sync</span></span>|
|<span data-ttu-id="b1205-118">dataquota</span><span class="sxs-lookup"><span data-stu-id="b1205-118">dataQuota</span></span>|<span data-ttu-id="b1205-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b1205-119">Int64</span></span>|<span data-ttu-id="b1205-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="b1205-120">Data quota</span></span>|
|<span data-ttu-id="b1205-121">dataused</span><span class="sxs-lookup"><span data-stu-id="b1205-121">dataUsed</span></span>|<span data-ttu-id="b1205-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b1205-122">Int64</span></span>|<span data-ttu-id="b1205-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="b1205-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1205-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b1205-124">Relationships</span></span>
<span data-ttu-id="b1205-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1205-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1205-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1205-126">JSON Representation</span></span>
<span data-ttu-id="b1205-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1205-127">Here is a JSON representation of the resource.</span></span>
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






