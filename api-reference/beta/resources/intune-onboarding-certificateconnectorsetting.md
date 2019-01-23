---
title: tipo de recurso de certificateConnectorSetting
description: Configurações do conector de certificado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398650"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="40be7-103">tipo de recurso de certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="40be7-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="40be7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="40be7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40be7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40be7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40be7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="40be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40be7-107">Configurações do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="40be7-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="40be7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40be7-108">Properties</span></span>
|<span data-ttu-id="40be7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40be7-109">Property</span></span>|<span data-ttu-id="40be7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="40be7-110">Type</span></span>|<span data-ttu-id="40be7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40be7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40be7-112">status</span><span class="sxs-lookup"><span data-stu-id="40be7-112">status</span></span>|<span data-ttu-id="40be7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="40be7-113">Int32</span></span>|<span data-ttu-id="40be7-114">Status do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="40be7-114">Certificate connector status</span></span>|
|<span data-ttu-id="40be7-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="40be7-115">certExpiryTime</span></span>|<span data-ttu-id="40be7-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40be7-116">DateTimeOffset</span></span>|<span data-ttu-id="40be7-117">Certificado expirará tempo</span><span class="sxs-lookup"><span data-stu-id="40be7-117">Certificate expire time</span></span>|
|<span data-ttu-id="40be7-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="40be7-118">enrollmentError</span></span>|<span data-ttu-id="40be7-119">String</span><span class="sxs-lookup"><span data-stu-id="40be7-119">String</span></span>|<span data-ttu-id="40be7-120">Erro de inscrição do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="40be7-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="40be7-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="40be7-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="40be7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40be7-122">DateTimeOffset</span></span>|<span data-ttu-id="40be7-123">Hora da última certificado conector conectado</span><span class="sxs-lookup"><span data-stu-id="40be7-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="40be7-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="40be7-124">connectorVersion</span></span>|<span data-ttu-id="40be7-125">String</span><span class="sxs-lookup"><span data-stu-id="40be7-125">String</span></span>|<span data-ttu-id="40be7-126">Versão do conector de certificado</span><span class="sxs-lookup"><span data-stu-id="40be7-126">Version of certificate connector</span></span>|
|<span data-ttu-id="40be7-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="40be7-127">lastUploadVersion</span></span>|<span data-ttu-id="40be7-128">Int64</span><span class="sxs-lookup"><span data-stu-id="40be7-128">Int64</span></span>|<span data-ttu-id="40be7-129">Versão do conector do último certificado carregado</span><span class="sxs-lookup"><span data-stu-id="40be7-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="40be7-130">Relações</span><span class="sxs-lookup"><span data-stu-id="40be7-130">Relationships</span></span>
<span data-ttu-id="40be7-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40be7-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40be7-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40be7-132">JSON Representation</span></span>
<span data-ttu-id="40be7-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40be7-133">Here is a JSON representation of the resource.</span></span>
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




