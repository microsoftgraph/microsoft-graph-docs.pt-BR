---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4dc78ad66302d4ffd330936cc95bd9b3cd7ae900
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383047"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="88fdc-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="88fdc-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="88fdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88fdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88fdc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88fdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88fdc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88fdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88fdc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="88fdc-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="88fdc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88fdc-108">Properties</span></span>
|<span data-ttu-id="88fdc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88fdc-109">Property</span></span>|<span data-ttu-id="88fdc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="88fdc-110">Type</span></span>|<span data-ttu-id="88fdc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="88fdc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88fdc-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88fdc-112">userPrincipalName</span></span>|<span data-ttu-id="88fdc-113">String</span><span class="sxs-lookup"><span data-stu-id="88fdc-113">String</span></span>|<span data-ttu-id="88fdc-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="88fdc-114">User name</span></span>|
|<span data-ttu-id="88fdc-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="88fdc-115">dataToSync</span></span>|<span data-ttu-id="88fdc-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="88fdc-116">Boolean</span></span>|<span data-ttu-id="88fdc-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="88fdc-117">Data to sync</span></span>|
|<span data-ttu-id="88fdc-118">dataquota</span><span class="sxs-lookup"><span data-stu-id="88fdc-118">dataQuota</span></span>|<span data-ttu-id="88fdc-119">Int64</span><span class="sxs-lookup"><span data-stu-id="88fdc-119">Int64</span></span>|<span data-ttu-id="88fdc-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="88fdc-120">Data quota</span></span>|
|<span data-ttu-id="88fdc-121">dataused</span><span class="sxs-lookup"><span data-stu-id="88fdc-121">dataUsed</span></span>|<span data-ttu-id="88fdc-122">Int64</span><span class="sxs-lookup"><span data-stu-id="88fdc-122">Int64</span></span>|<span data-ttu-id="88fdc-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="88fdc-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="88fdc-124">Relações</span><span class="sxs-lookup"><span data-stu-id="88fdc-124">Relationships</span></span>
<span data-ttu-id="88fdc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88fdc-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88fdc-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88fdc-126">JSON Representation</span></span>
<span data-ttu-id="88fdc-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88fdc-127">Here is a JSON representation of the resource.</span></span>
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



