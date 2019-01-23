---
title: tipo de recurso de sharedAppleDeviceUser
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46e0993c69a8ae34a54a654959d8d67a1b7f4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394429"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="19c43-103">tipo de recurso de sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="19c43-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="19c43-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="19c43-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19c43-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19c43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19c43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="19c43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c43-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="19c43-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="19c43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19c43-108">Properties</span></span>
|<span data-ttu-id="19c43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19c43-109">Property</span></span>|<span data-ttu-id="19c43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="19c43-110">Type</span></span>|<span data-ttu-id="19c43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19c43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c43-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19c43-112">userPrincipalName</span></span>|<span data-ttu-id="19c43-113">String</span><span class="sxs-lookup"><span data-stu-id="19c43-113">String</span></span>|<span data-ttu-id="19c43-114">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="19c43-114">User name</span></span>|
|<span data-ttu-id="19c43-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="19c43-115">dataToSync</span></span>|<span data-ttu-id="19c43-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="19c43-116">Boolean</span></span>|<span data-ttu-id="19c43-117">Dados a serem sincronizados</span><span class="sxs-lookup"><span data-stu-id="19c43-117">Data to sync</span></span>|
|<span data-ttu-id="19c43-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="19c43-118">dataQuota</span></span>|<span data-ttu-id="19c43-119">Int64</span><span class="sxs-lookup"><span data-stu-id="19c43-119">Int64</span></span>|<span data-ttu-id="19c43-120">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="19c43-120">Data quota</span></span>|
|<span data-ttu-id="19c43-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="19c43-121">dataUsed</span></span>|<span data-ttu-id="19c43-122">Int64</span><span class="sxs-lookup"><span data-stu-id="19c43-122">Int64</span></span>|<span data-ttu-id="19c43-123">Cota de dados</span><span class="sxs-lookup"><span data-stu-id="19c43-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c43-124">Relações</span><span class="sxs-lookup"><span data-stu-id="19c43-124">Relationships</span></span>
<span data-ttu-id="19c43-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19c43-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19c43-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19c43-126">JSON Representation</span></span>
<span data-ttu-id="19c43-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19c43-127">Here is a JSON representation of the resource.</span></span>
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




