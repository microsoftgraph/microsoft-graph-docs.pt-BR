---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3946247ba9424fb1c961a11753376b7bcfb78c4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724449"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="6bc46-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="6bc46-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="6bc46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bc46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bc46-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6bc46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bc46-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bc46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bc46-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6bc46-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6bc46-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bc46-108">Properties</span></span>
|<span data-ttu-id="6bc46-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bc46-109">Property</span></span>|<span data-ttu-id="6bc46-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bc46-110">Type</span></span>|<span data-ttu-id="6bc46-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bc46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc46-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6bc46-112">userPrincipalName</span></span>|<span data-ttu-id="6bc46-113">String</span><span class="sxs-lookup"><span data-stu-id="6bc46-113">String</span></span>|<span data-ttu-id="6bc46-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="6bc46-114">User name</span></span>|
|<span data-ttu-id="6bc46-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="6bc46-115">dataToSync</span></span>|<span data-ttu-id="6bc46-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="6bc46-116">Boolean</span></span>|<span data-ttu-id="6bc46-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="6bc46-117">Data to sync</span></span>|
|<span data-ttu-id="6bc46-118">dataquota</span><span class="sxs-lookup"><span data-stu-id="6bc46-118">dataQuota</span></span>|<span data-ttu-id="6bc46-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6bc46-119">Int64</span></span>|<span data-ttu-id="6bc46-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="6bc46-120">Data quota</span></span>|
|<span data-ttu-id="6bc46-121">dataused</span><span class="sxs-lookup"><span data-stu-id="6bc46-121">dataUsed</span></span>|<span data-ttu-id="6bc46-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6bc46-122">Int64</span></span>|<span data-ttu-id="6bc46-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="6bc46-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bc46-124">Relações</span><span class="sxs-lookup"><span data-stu-id="6bc46-124">Relationships</span></span>
<span data-ttu-id="6bc46-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bc46-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bc46-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bc46-126">JSON Representation</span></span>
<span data-ttu-id="6bc46-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6bc46-127">Here is a JSON representation of the resource.</span></span>
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





