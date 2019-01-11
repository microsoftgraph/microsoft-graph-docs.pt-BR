---
title: tipo de recurso de certificateConnectorSetting
description: Configurações do conector de certificado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888596"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="9e6e6-103">tipo de recurso de certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="9e6e6-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="9e6e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e6e6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e6e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e6e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e6e6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9e6e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e6e6-107">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="9e6e6-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="9e6e6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e6e6-108">Properties</span></span>
|<span data-ttu-id="9e6e6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e6e6-109">Property</span></span>|<span data-ttu-id="9e6e6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e6e6-110">Type</span></span>|<span data-ttu-id="9e6e6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e6e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e6e6-112">status</span><span class="sxs-lookup"><span data-stu-id="9e6e6-112">status</span></span>|<span data-ttu-id="9e6e6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9e6e6-113">Int32</span></span>|<span data-ttu-id="9e6e6-114">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="9e6e6-114">Certificate connector status</span></span>|
|<span data-ttu-id="9e6e6-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="9e6e6-115">certExpiryTime</span></span>|<span data-ttu-id="9e6e6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6e6-116">DateTimeOffset</span></span>|<span data-ttu-id="9e6e6-117">Certificado expirará tempo</span><span class="sxs-lookup"><span data-stu-id="9e6e6-117">Certificate expire time</span></span>|
|<span data-ttu-id="9e6e6-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="9e6e6-118">enrollmentError</span></span>|<span data-ttu-id="9e6e6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e6e6-119">String</span></span>|<span data-ttu-id="9e6e6-120">Erro de inscrição do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="9e6e6-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="9e6e6-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="9e6e6-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="9e6e6-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6e6-122">DateTimeOffset</span></span>|<span data-ttu-id="9e6e6-123">Hora da última certificado conector conectado</span><span class="sxs-lookup"><span data-stu-id="9e6e6-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="9e6e6-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="9e6e6-124">connectorVersion</span></span>|<span data-ttu-id="9e6e6-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e6e6-125">String</span></span>|<span data-ttu-id="9e6e6-126">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="9e6e6-126">Version of certificate connector</span></span>|
|<span data-ttu-id="9e6e6-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="9e6e6-127">lastUploadVersion</span></span>|<span data-ttu-id="9e6e6-128">Int64</span><span class="sxs-lookup"><span data-stu-id="9e6e6-128">Int64</span></span>|<span data-ttu-id="9e6e6-129">Versão do conector do último certificado carregado</span><span class="sxs-lookup"><span data-stu-id="9e6e6-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e6e6-130">Relações</span><span class="sxs-lookup"><span data-stu-id="9e6e6-130">Relationships</span></span>
<span data-ttu-id="9e6e6-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e6e6-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e6e6-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e6e6-132">JSON Representation</span></span>
<span data-ttu-id="9e6e6-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e6e6-133">Here is a JSON representation of the resource.</span></span>
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





