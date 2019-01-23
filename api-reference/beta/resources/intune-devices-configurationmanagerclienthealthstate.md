---
title: tipo de recurso de configurationManagerClientHealthState
description: Estado de integridade de cliente do Configuration manager
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425824"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="ba0d5-103">tipo de recurso de configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ba0d5-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="ba0d5-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba0d5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba0d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba0d5-107">Estado de integridade de cliente do Configuration manager</span><span class="sxs-lookup"><span data-stu-id="ba0d5-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="ba0d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba0d5-108">Properties</span></span>
|<span data-ttu-id="ba0d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba0d5-109">Property</span></span>|<span data-ttu-id="ba0d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba0d5-110">Type</span></span>|<span data-ttu-id="ba0d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba0d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba0d5-112">state</span><span class="sxs-lookup"><span data-stu-id="ba0d5-112">state</span></span>|[<span data-ttu-id="ba0d5-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="ba0d5-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="ba0d5-114">Estado da cliente do Gerenciador de configuração atual.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-114">Current configuration manager client state.</span></span> <span data-ttu-id="ba0d5-115">Os valores possíveis são: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="ba0d5-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="ba0d5-116">errorCode</span></span>|<span data-ttu-id="ba0d5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ba0d5-117">Int32</span></span>|<span data-ttu-id="ba0d5-118">Código de erro para o estado de falha.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-118">Error code for failed state.</span></span>|
|<span data-ttu-id="ba0d5-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ba0d5-119">lastSyncDateTime</span></span>|<span data-ttu-id="ba0d5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba0d5-120">DateTimeOffset</span></span>|<span data-ttu-id="ba0d5-121">Ponto de DateTime fo última sincronização com o gerenciamento do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba0d5-122">Relações</span><span class="sxs-lookup"><span data-stu-id="ba0d5-122">Relationships</span></span>
<span data-ttu-id="ba0d5-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba0d5-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba0d5-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba0d5-124">JSON Representation</span></span>
<span data-ttu-id="ba0d5-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba0d5-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```




