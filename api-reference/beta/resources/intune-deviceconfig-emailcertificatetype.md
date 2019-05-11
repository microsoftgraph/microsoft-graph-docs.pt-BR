---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 150109f68d4cac95c07d2bc973149b1309fefc07
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33956882"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="21954-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="21954-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="21954-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21954-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21954-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21954-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21954-106">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="21954-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="21954-107">Membros</span><span class="sxs-lookup"><span data-stu-id="21954-107">Members</span></span>
|<span data-ttu-id="21954-108">Membro</span><span class="sxs-lookup"><span data-stu-id="21954-108">Member</span></span>|<span data-ttu-id="21954-109">Valor</span><span class="sxs-lookup"><span data-stu-id="21954-109">Value</span></span>|<span data-ttu-id="21954-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21954-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21954-111">none</span><span class="sxs-lookup"><span data-stu-id="21954-111">none</span></span>|<span data-ttu-id="21954-112">,0</span><span class="sxs-lookup"><span data-stu-id="21954-112">0</span></span>|<span data-ttu-id="21954-113">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="21954-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="21954-114">certificado</span><span class="sxs-lookup"><span data-stu-id="21954-114">certificate</span></span>|<span data-ttu-id="21954-115">1</span><span class="sxs-lookup"><span data-stu-id="21954-115">1</span></span>|<span data-ttu-id="21954-116">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="21954-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="21954-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="21954-117">derivedCredential</span></span>|<span data-ttu-id="21954-118">duas</span><span class="sxs-lookup"><span data-stu-id="21954-118">2</span></span>|<span data-ttu-id="21954-119">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="21954-119">Use a derived credential for certificate source.</span></span>|




