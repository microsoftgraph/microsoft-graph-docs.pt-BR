---
title: tipo de recurso de deviceManagementExchangeAccessRule
description: Regras de acesso de dispositivo no Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409437"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="1dcf2-103">tipo de recurso de deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="1dcf2-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="1dcf2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1dcf2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dcf2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dcf2-107">Regras de acesso de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="1dcf2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dcf2-108">Properties</span></span>
|<span data-ttu-id="1dcf2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dcf2-109">Property</span></span>|<span data-ttu-id="1dcf2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dcf2-110">Type</span></span>|<span data-ttu-id="1dcf2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dcf2-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="1dcf2-112">deviceClass</span></span>|[<span data-ttu-id="1dcf2-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="1dcf2-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="1dcf2-114">Classe de dispositivo que será afetado por essa regra.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="1dcf2-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="1dcf2-115">accessLevel</span></span>|[<span data-ttu-id="1dcf2-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="1dcf2-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="1dcf2-117">Nível de acesso para o Exchange concedida por esta regra.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="1dcf2-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dcf2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1dcf2-119">Relationships</span></span>
<span data-ttu-id="1dcf2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dcf2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dcf2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dcf2-121">JSON Representation</span></span>
<span data-ttu-id="1dcf2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dcf2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```




