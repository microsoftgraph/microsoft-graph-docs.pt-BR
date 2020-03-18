---
title: tipo de recurso sharedAppleDeviceUser
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 550d8af3cab51f611feed7f87f1d2f56a850de4e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783855"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="caa87-103">tipo de recurso sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="caa87-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="caa87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="caa87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caa87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="caa87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caa87-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="caa87-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="caa87-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="caa87-107">Properties</span></span>
|<span data-ttu-id="caa87-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="caa87-108">Property</span></span>|<span data-ttu-id="caa87-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="caa87-109">Type</span></span>|<span data-ttu-id="caa87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="caa87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caa87-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="caa87-111">userPrincipalName</span></span>|<span data-ttu-id="caa87-112">String</span><span class="sxs-lookup"><span data-stu-id="caa87-112">String</span></span>|<span data-ttu-id="caa87-113">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="caa87-113">User name</span></span>|
|<span data-ttu-id="caa87-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="caa87-114">dataToSync</span></span>|<span data-ttu-id="caa87-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="caa87-115">Boolean</span></span>|<span data-ttu-id="caa87-116">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="caa87-116">Data to sync</span></span>|
|<span data-ttu-id="caa87-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="caa87-117">dataQuota</span></span>|<span data-ttu-id="caa87-118">Int64</span><span class="sxs-lookup"><span data-stu-id="caa87-118">Int64</span></span>|<span data-ttu-id="caa87-119">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="caa87-119">Data quota</span></span>|
|<span data-ttu-id="caa87-120">dataused</span><span class="sxs-lookup"><span data-stu-id="caa87-120">dataUsed</span></span>|<span data-ttu-id="caa87-121">Int64</span><span class="sxs-lookup"><span data-stu-id="caa87-121">Int64</span></span>|<span data-ttu-id="caa87-122">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="caa87-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="caa87-123">Relações</span><span class="sxs-lookup"><span data-stu-id="caa87-123">Relationships</span></span>
<span data-ttu-id="caa87-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caa87-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="caa87-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="caa87-125">JSON Representation</span></span>
<span data-ttu-id="caa87-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="caa87-126">Here is a JSON representation of the resource.</span></span>
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



