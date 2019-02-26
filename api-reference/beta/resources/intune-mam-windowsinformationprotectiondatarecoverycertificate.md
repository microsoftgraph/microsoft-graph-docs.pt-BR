---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c480b8117f3d8dbf0ad8208bac09b63b113906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156186"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="f9984-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="f9984-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="f9984-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9984-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9984-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9984-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9984-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="f9984-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="f9984-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9984-107">Properties</span></span>
|<span data-ttu-id="f9984-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9984-108">Property</span></span>|<span data-ttu-id="f9984-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9984-109">Type</span></span>|<span data-ttu-id="f9984-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9984-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9984-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="f9984-111">subjectName</span></span>|<span data-ttu-id="f9984-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9984-112">String</span></span>|<span data-ttu-id="f9984-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="f9984-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="f9984-114">descrição</span><span class="sxs-lookup"><span data-stu-id="f9984-114">description</span></span>|<span data-ttu-id="f9984-115">String</span><span class="sxs-lookup"><span data-stu-id="f9984-115">String</span></span>|<span data-ttu-id="f9984-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="f9984-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="f9984-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9984-117">expirationDateTime</span></span>|<span data-ttu-id="f9984-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9984-118">DateTimeOffset</span></span>|<span data-ttu-id="f9984-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="f9984-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="f9984-120">certificado</span><span class="sxs-lookup"><span data-stu-id="f9984-120">certificate</span></span>|<span data-ttu-id="f9984-121">Binário</span><span class="sxs-lookup"><span data-stu-id="f9984-121">Binary</span></span>|<span data-ttu-id="f9984-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="f9984-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9984-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f9984-123">Relationships</span></span>
<span data-ttu-id="f9984-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9984-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9984-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9984-125">JSON Representation</span></span>
<span data-ttu-id="f9984-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9984-126">Here is a JSON representation of the resource.</span></span>
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




