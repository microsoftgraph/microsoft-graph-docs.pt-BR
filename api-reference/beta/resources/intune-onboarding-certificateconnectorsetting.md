---
title: tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014d9ab627d1606d9850548128c51ed52939f2c8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995536"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="54d78-103">tipo de recurso certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="54d78-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="54d78-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54d78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54d78-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54d78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54d78-106">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="54d78-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="54d78-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54d78-107">Properties</span></span>
|<span data-ttu-id="54d78-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54d78-108">Property</span></span>|<span data-ttu-id="54d78-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="54d78-109">Type</span></span>|<span data-ttu-id="54d78-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54d78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d78-111">status</span><span class="sxs-lookup"><span data-stu-id="54d78-111">status</span></span>|<span data-ttu-id="54d78-112">Int32</span><span class="sxs-lookup"><span data-stu-id="54d78-112">Int32</span></span>|<span data-ttu-id="54d78-113">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="54d78-113">Certificate connector status</span></span>|
|<span data-ttu-id="54d78-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="54d78-114">certExpiryTime</span></span>|<span data-ttu-id="54d78-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d78-115">DateTimeOffset</span></span>|<span data-ttu-id="54d78-116">Tempo de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="54d78-116">Certificate expire time</span></span>|
|<span data-ttu-id="54d78-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="54d78-117">enrollmentError</span></span>|<span data-ttu-id="54d78-118">String</span><span class="sxs-lookup"><span data-stu-id="54d78-118">String</span></span>|<span data-ttu-id="54d78-119">Erro de registro do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="54d78-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="54d78-120">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="54d78-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="54d78-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54d78-121">DateTimeOffset</span></span>|<span data-ttu-id="54d78-122">Última vez em que o conector de certificado está conectado</span><span class="sxs-lookup"><span data-stu-id="54d78-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="54d78-123">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="54d78-123">connectorVersion</span></span>|<span data-ttu-id="54d78-124">String</span><span class="sxs-lookup"><span data-stu-id="54d78-124">String</span></span>|<span data-ttu-id="54d78-125">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="54d78-125">Version of certificate connector</span></span>|
|<span data-ttu-id="54d78-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="54d78-126">lastUploadVersion</span></span>|<span data-ttu-id="54d78-127">Int64</span><span class="sxs-lookup"><span data-stu-id="54d78-127">Int64</span></span>|<span data-ttu-id="54d78-128">Versão do último conector de certificado carregado</span><span class="sxs-lookup"><span data-stu-id="54d78-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="54d78-129">Relações</span><span class="sxs-lookup"><span data-stu-id="54d78-129">Relationships</span></span>
<span data-ttu-id="54d78-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54d78-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54d78-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54d78-131">JSON Representation</span></span>
<span data-ttu-id="54d78-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54d78-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





