---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1da5da59fb0b3b2485ed2dd22710e13f64307843
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984373"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="49eeb-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="49eeb-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="49eeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49eeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49eeb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49eeb-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="49eeb-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="49eeb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49eeb-107">Properties</span></span>
|<span data-ttu-id="49eeb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49eeb-108">Property</span></span>|<span data-ttu-id="49eeb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="49eeb-109">Type</span></span>|<span data-ttu-id="49eeb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49eeb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49eeb-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="49eeb-111">subjectName</span></span>|<span data-ttu-id="49eeb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49eeb-112">String</span></span>|<span data-ttu-id="49eeb-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="49eeb-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="49eeb-114">description</span><span class="sxs-lookup"><span data-stu-id="49eeb-114">description</span></span>|<span data-ttu-id="49eeb-115">String</span><span class="sxs-lookup"><span data-stu-id="49eeb-115">String</span></span>|<span data-ttu-id="49eeb-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="49eeb-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="49eeb-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49eeb-117">expirationDateTime</span></span>|<span data-ttu-id="49eeb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49eeb-118">DateTimeOffset</span></span>|<span data-ttu-id="49eeb-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="49eeb-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="49eeb-120">certificado</span><span class="sxs-lookup"><span data-stu-id="49eeb-120">certificate</span></span>|<span data-ttu-id="49eeb-121">Binário</span><span class="sxs-lookup"><span data-stu-id="49eeb-121">Binary</span></span>|<span data-ttu-id="49eeb-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="49eeb-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="49eeb-123">Relações</span><span class="sxs-lookup"><span data-stu-id="49eeb-123">Relationships</span></span>
<span data-ttu-id="49eeb-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49eeb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49eeb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49eeb-125">JSON Representation</span></span>
<span data-ttu-id="49eeb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49eeb-126">Here is a JSON representation of the resource.</span></span>
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









