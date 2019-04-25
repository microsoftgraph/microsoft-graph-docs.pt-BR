---
title: tipo de recurso certificateConnectorSetting
description: Configurações do conector de certificado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe154ed3150ae434f8068bc04a56dd6e5b48744
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573057"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="37d5e-103">tipo de recurso certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="37d5e-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="37d5e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37d5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37d5e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37d5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37d5e-106">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="37d5e-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="37d5e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37d5e-107">Properties</span></span>
|<span data-ttu-id="37d5e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37d5e-108">Property</span></span>|<span data-ttu-id="37d5e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37d5e-109">Type</span></span>|<span data-ttu-id="37d5e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d5e-111">status</span><span class="sxs-lookup"><span data-stu-id="37d5e-111">status</span></span>|<span data-ttu-id="37d5e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="37d5e-112">Int32</span></span>|<span data-ttu-id="37d5e-113">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="37d5e-113">Certificate connector status</span></span>|
|<span data-ttu-id="37d5e-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="37d5e-114">certExpiryTime</span></span>|<span data-ttu-id="37d5e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d5e-115">DateTimeOffset</span></span>|<span data-ttu-id="37d5e-116">Tempo de validade do certificado</span><span class="sxs-lookup"><span data-stu-id="37d5e-116">Certificate expire time</span></span>|
|<span data-ttu-id="37d5e-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="37d5e-117">enrollmentError</span></span>|<span data-ttu-id="37d5e-118">String</span><span class="sxs-lookup"><span data-stu-id="37d5e-118">String</span></span>|<span data-ttu-id="37d5e-119">Erro de registro do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="37d5e-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="37d5e-120">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="37d5e-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="37d5e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d5e-121">DateTimeOffset</span></span>|<span data-ttu-id="37d5e-122">Última vez em que o conector de certificado está conectado</span><span class="sxs-lookup"><span data-stu-id="37d5e-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="37d5e-123">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="37d5e-123">connectorVersion</span></span>|<span data-ttu-id="37d5e-124">String</span><span class="sxs-lookup"><span data-stu-id="37d5e-124">String</span></span>|<span data-ttu-id="37d5e-125">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="37d5e-125">Version of certificate connector</span></span>|
|<span data-ttu-id="37d5e-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="37d5e-126">lastUploadVersion</span></span>|<span data-ttu-id="37d5e-127">Int64</span><span class="sxs-lookup"><span data-stu-id="37d5e-127">Int64</span></span>|<span data-ttu-id="37d5e-128">Versão do último conector de certificado carregado</span><span class="sxs-lookup"><span data-stu-id="37d5e-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="37d5e-129">Relações</span><span class="sxs-lookup"><span data-stu-id="37d5e-129">Relationships</span></span>
<span data-ttu-id="37d5e-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37d5e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37d5e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37d5e-131">JSON Representation</span></span>
<span data-ttu-id="37d5e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37d5e-132">Here is a JSON representation of the resource.</span></span>
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





