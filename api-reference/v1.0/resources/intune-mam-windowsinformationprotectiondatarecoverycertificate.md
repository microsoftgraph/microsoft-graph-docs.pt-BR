---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a62c0351b3247300e47c8c9a91aecbc32092e015
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367319"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8b8ff-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8b8ff-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="8b8ff-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b8ff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b8ff-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="8b8ff-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="8b8ff-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b8ff-106">Properties</span></span>
|<span data-ttu-id="8b8ff-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b8ff-107">Property</span></span>|<span data-ttu-id="8b8ff-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b8ff-108">Type</span></span>|<span data-ttu-id="8b8ff-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b8ff-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b8ff-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8b8ff-110">subjectName</span></span>|<span data-ttu-id="8b8ff-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b8ff-111">String</span></span>|<span data-ttu-id="8b8ff-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8b8ff-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8b8ff-113">descrição</span><span class="sxs-lookup"><span data-stu-id="8b8ff-113">description</span></span>|<span data-ttu-id="8b8ff-114">String</span><span class="sxs-lookup"><span data-stu-id="8b8ff-114">String</span></span>|<span data-ttu-id="8b8ff-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8b8ff-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8b8ff-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8b8ff-116">expirationDateTime</span></span>|<span data-ttu-id="8b8ff-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b8ff-117">DateTimeOffset</span></span>|<span data-ttu-id="8b8ff-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8b8ff-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8b8ff-119">certificado</span><span class="sxs-lookup"><span data-stu-id="8b8ff-119">certificate</span></span>|<span data-ttu-id="8b8ff-120">Binário</span><span class="sxs-lookup"><span data-stu-id="8b8ff-120">Binary</span></span>|<span data-ttu-id="8b8ff-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8b8ff-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b8ff-122">Relações</span><span class="sxs-lookup"><span data-stu-id="8b8ff-122">Relationships</span></span>
<span data-ttu-id="8b8ff-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b8ff-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b8ff-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b8ff-124">JSON Representation</span></span>
<span data-ttu-id="8b8ff-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b8ff-125">Here is a JSON representation of the resource.</span></span>
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




