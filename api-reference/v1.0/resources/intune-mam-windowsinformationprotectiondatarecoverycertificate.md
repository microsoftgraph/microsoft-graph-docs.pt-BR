---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a23a05a53170929712d4cfd8c4dd9f634fba5dc4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751276"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="d19ab-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d19ab-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="d19ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d19ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d19ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d19ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d19ab-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="d19ab-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="d19ab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d19ab-107">Properties</span></span>
|<span data-ttu-id="d19ab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d19ab-108">Property</span></span>|<span data-ttu-id="d19ab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19ab-109">Type</span></span>|<span data-ttu-id="d19ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d19ab-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="d19ab-111">subjectName</span></span>|<span data-ttu-id="d19ab-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d19ab-112">String</span></span>|<span data-ttu-id="d19ab-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="d19ab-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="d19ab-114">descrição</span><span class="sxs-lookup"><span data-stu-id="d19ab-114">description</span></span>|<span data-ttu-id="d19ab-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d19ab-115">String</span></span>|<span data-ttu-id="d19ab-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="d19ab-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="d19ab-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d19ab-117">expirationDateTime</span></span>|<span data-ttu-id="d19ab-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d19ab-118">DateTimeOffset</span></span>|<span data-ttu-id="d19ab-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="d19ab-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="d19ab-120">certificado</span><span class="sxs-lookup"><span data-stu-id="d19ab-120">certificate</span></span>|<span data-ttu-id="d19ab-121">Binário</span><span class="sxs-lookup"><span data-stu-id="d19ab-121">Binary</span></span>|<span data-ttu-id="d19ab-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="d19ab-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d19ab-123">Relações</span><span class="sxs-lookup"><span data-stu-id="d19ab-123">Relationships</span></span>
<span data-ttu-id="d19ab-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d19ab-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d19ab-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d19ab-125">JSON Representation</span></span>
<span data-ttu-id="d19ab-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d19ab-126">Here is a JSON representation of the resource.</span></span>
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




