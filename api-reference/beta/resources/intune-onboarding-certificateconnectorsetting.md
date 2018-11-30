---
title: tipo de recurso de certificateConnectorSetting
description: Configurações do conector de certificado.
ms.openlocfilehash: 65f87002016c4d5bd6b19106ba1aa988ad30d92e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032901"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="91b6b-103">tipo de recurso de certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="91b6b-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="91b6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91b6b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91b6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91b6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91b6b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91b6b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91b6b-107">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="91b6b-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="91b6b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91b6b-108">Properties</span></span>
|<span data-ttu-id="91b6b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91b6b-109">Property</span></span>|<span data-ttu-id="91b6b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b6b-110">Type</span></span>|<span data-ttu-id="91b6b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b6b-112">status</span><span class="sxs-lookup"><span data-stu-id="91b6b-112">status</span></span>|<span data-ttu-id="91b6b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="91b6b-113">Int32</span></span>|<span data-ttu-id="91b6b-114">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="91b6b-114">Certificate connector status</span></span>|
|<span data-ttu-id="91b6b-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="91b6b-115">certExpiryTime</span></span>|<span data-ttu-id="91b6b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91b6b-116">DateTimeOffset</span></span>|<span data-ttu-id="91b6b-117">Certificado expirará tempo</span><span class="sxs-lookup"><span data-stu-id="91b6b-117">Certificate expire time</span></span>|
|<span data-ttu-id="91b6b-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="91b6b-118">enrollmentError</span></span>|<span data-ttu-id="91b6b-119">String</span><span class="sxs-lookup"><span data-stu-id="91b6b-119">String</span></span>|<span data-ttu-id="91b6b-120">Erro de inscrição do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="91b6b-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="91b6b-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="91b6b-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="91b6b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91b6b-122">DateTimeOffset</span></span>|<span data-ttu-id="91b6b-123">Hora da última certificado conector conectado</span><span class="sxs-lookup"><span data-stu-id="91b6b-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="91b6b-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="91b6b-124">connectorVersion</span></span>|<span data-ttu-id="91b6b-125">String</span><span class="sxs-lookup"><span data-stu-id="91b6b-125">String</span></span>|<span data-ttu-id="91b6b-126">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="91b6b-126">Version of certificate connector</span></span>|
|<span data-ttu-id="91b6b-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="91b6b-127">lastUploadVersion</span></span>|<span data-ttu-id="91b6b-128">Int64</span><span class="sxs-lookup"><span data-stu-id="91b6b-128">Int64</span></span>|<span data-ttu-id="91b6b-129">Versão do conector do último certificado carregado</span><span class="sxs-lookup"><span data-stu-id="91b6b-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b6b-130">Relações</span><span class="sxs-lookup"><span data-stu-id="91b6b-130">Relationships</span></span>
<span data-ttu-id="91b6b-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91b6b-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91b6b-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91b6b-132">JSON Representation</span></span>
<span data-ttu-id="91b6b-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91b6b-133">Here is a JSON representation of the resource.</span></span>
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





