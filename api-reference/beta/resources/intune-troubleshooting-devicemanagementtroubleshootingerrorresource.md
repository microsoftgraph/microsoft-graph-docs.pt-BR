---
title: tipo de recurso de deviceManagementTroubleshootingErrorResource
description: Objeto que representa um link para obter informações, o link de solução de problemas poderia ser o Portal do Windows Azure ou um doc da Microsoft.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429250"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="b4729-103">tipo de recurso de deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="b4729-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="b4729-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4729-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4729-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4729-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4729-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b4729-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4729-107">Objeto que representa um link para obter informações, o link de solução de problemas poderia ser o Portal do Windows Azure ou um doc da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b4729-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="b4729-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4729-108">Properties</span></span>
|<span data-ttu-id="b4729-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4729-109">Property</span></span>|<span data-ttu-id="b4729-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4729-110">Type</span></span>|<span data-ttu-id="b4729-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4729-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4729-112">texto</span><span class="sxs-lookup"><span data-stu-id="b4729-112">text</span></span>|<span data-ttu-id="b4729-113">String</span><span class="sxs-lookup"><span data-stu-id="b4729-113">String</span></span>|<span data-ttu-id="b4729-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4729-114">Not yet documented</span></span>|
|<span data-ttu-id="b4729-115">vínculo</span><span class="sxs-lookup"><span data-stu-id="b4729-115">link</span></span>|<span data-ttu-id="b4729-116">String</span><span class="sxs-lookup"><span data-stu-id="b4729-116">String</span></span>|<span data-ttu-id="b4729-117">O link para o recurso da web.</span><span class="sxs-lookup"><span data-stu-id="b4729-117">The link to the web resource.</span></span> <span data-ttu-id="b4729-118">Pode conter qualquer um dos formatadores a seguir: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="b4729-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4729-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b4729-119">Relationships</span></span>
<span data-ttu-id="b4729-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4729-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4729-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4729-121">JSON Representation</span></span>
<span data-ttu-id="b4729-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4729-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




