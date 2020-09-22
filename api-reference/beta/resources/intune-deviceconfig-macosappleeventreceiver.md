---
title: tipo de recurso macOSAppleEventReceiver
description: Representa um processo que pode receber uma notificação de evento Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db781ad536e8fe918257f74d87fa104f4b2a23f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055446"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="7a8bc-103">tipo de recurso macOSAppleEventReceiver</span><span class="sxs-lookup"><span data-stu-id="7a8bc-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="7a8bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a8bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a8bc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a8bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a8bc-107">Representa um processo que pode receber uma notificação de evento Apple.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="7a8bc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8bc-108">Properties</span></span>
|<span data-ttu-id="7a8bc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8bc-109">Property</span></span>|<span data-ttu-id="7a8bc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8bc-110">Type</span></span>|<span data-ttu-id="7a8bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8bc-112">codeRequirement</span><span class="sxs-lookup"><span data-stu-id="7a8bc-112">codeRequirement</span></span>|<span data-ttu-id="7a8bc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8bc-113">String</span></span>|<span data-ttu-id="7a8bc-114">Requisito de código para o aplicativo ou o binário que recebe o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="7a8bc-115">identificador</span><span class="sxs-lookup"><span data-stu-id="7a8bc-115">identifier</span></span>|<span data-ttu-id="7a8bc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8bc-116">String</span></span>|<span data-ttu-id="7a8bc-117">ID de pacote do aplicativo ou caminho de arquivo do processo ou executável que recebe o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="7a8bc-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="7a8bc-118">identifierType</span></span>|[<span data-ttu-id="7a8bc-119">macOSProcessIdentifierType</span><span class="sxs-lookup"><span data-stu-id="7a8bc-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="7a8bc-120">Use ID de pacote para um aplicativo ou caminho para um processo ou executável que receba o evento Apple.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="7a8bc-121">Os valores possíveis são: `bundleID` e `path`.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="7a8bc-122">autorizado</span><span class="sxs-lookup"><span data-stu-id="7a8bc-122">allowed</span></span>|<span data-ttu-id="7a8bc-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="7a8bc-123">Boolean</span></span>|<span data-ttu-id="7a8bc-124">Permitir ou impedir que este aplicativo receba eventos Apple.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a8bc-125">Relações</span><span class="sxs-lookup"><span data-stu-id="7a8bc-125">Relationships</span></span>
<span data-ttu-id="7a8bc-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a8bc-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a8bc-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8bc-127">JSON Representation</span></span>
<span data-ttu-id="7a8bc-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a8bc-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```






