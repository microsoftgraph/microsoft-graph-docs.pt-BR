---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5d755ed3b8a1bfb34df3702168abb3ad589474c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524262"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="890bb-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="890bb-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="890bb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="890bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="890bb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="890bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="890bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="890bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="890bb-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="890bb-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="890bb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="890bb-108">Properties</span></span>
|<span data-ttu-id="890bb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="890bb-109">Property</span></span>|<span data-ttu-id="890bb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="890bb-110">Type</span></span>|<span data-ttu-id="890bb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="890bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890bb-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="890bb-112">subjectName</span></span>|<span data-ttu-id="890bb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="890bb-113">String</span></span>|<span data-ttu-id="890bb-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="890bb-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="890bb-115">description</span><span class="sxs-lookup"><span data-stu-id="890bb-115">description</span></span>|<span data-ttu-id="890bb-116">String</span><span class="sxs-lookup"><span data-stu-id="890bb-116">String</span></span>|<span data-ttu-id="890bb-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="890bb-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="890bb-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="890bb-118">expirationDateTime</span></span>|<span data-ttu-id="890bb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890bb-119">DateTimeOffset</span></span>|<span data-ttu-id="890bb-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="890bb-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="890bb-121">certificado</span><span class="sxs-lookup"><span data-stu-id="890bb-121">certificate</span></span>|<span data-ttu-id="890bb-122">Binário</span><span class="sxs-lookup"><span data-stu-id="890bb-122">Binary</span></span>|<span data-ttu-id="890bb-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="890bb-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="890bb-124">Relações</span><span class="sxs-lookup"><span data-stu-id="890bb-124">Relationships</span></span>
<span data-ttu-id="890bb-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="890bb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="890bb-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="890bb-126">JSON Representation</span></span>
<span data-ttu-id="890bb-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="890bb-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



