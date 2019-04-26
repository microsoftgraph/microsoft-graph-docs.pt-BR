---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561184"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8f865-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8f865-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="8f865-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f865-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f865-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="8f865-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="8f865-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f865-106">Properties</span></span>
|<span data-ttu-id="8f865-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f865-107">Property</span></span>|<span data-ttu-id="8f865-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f865-108">Type</span></span>|<span data-ttu-id="8f865-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f865-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f865-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="8f865-110">subjectName</span></span>|<span data-ttu-id="8f865-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f865-111">String</span></span>|<span data-ttu-id="8f865-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8f865-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8f865-113">description</span><span class="sxs-lookup"><span data-stu-id="8f865-113">description</span></span>|<span data-ttu-id="8f865-114">String</span><span class="sxs-lookup"><span data-stu-id="8f865-114">String</span></span>|<span data-ttu-id="8f865-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8f865-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8f865-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8f865-116">expirationDateTime</span></span>|<span data-ttu-id="8f865-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f865-117">DateTimeOffset</span></span>|<span data-ttu-id="8f865-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8f865-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8f865-119">certificado</span><span class="sxs-lookup"><span data-stu-id="8f865-119">certificate</span></span>|<span data-ttu-id="8f865-120">Binário</span><span class="sxs-lookup"><span data-stu-id="8f865-120">Binary</span></span>|<span data-ttu-id="8f865-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="8f865-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f865-122">Relações</span><span class="sxs-lookup"><span data-stu-id="8f865-122">Relationships</span></span>
<span data-ttu-id="8f865-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f865-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f865-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f865-124">JSON Representation</span></span>
<span data-ttu-id="8f865-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f865-125">Here is a JSON representation of the resource.</span></span>
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



