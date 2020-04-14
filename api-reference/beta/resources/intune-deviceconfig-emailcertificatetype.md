---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d2f5e4add7f67c6b772aa903d4e3b860b67ecbf5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460098"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="44ba1-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="44ba1-103">emailCertificateType enum type</span></span>

<span data-ttu-id="44ba1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44ba1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44ba1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44ba1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ba1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44ba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ba1-107">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="44ba1-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="44ba1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="44ba1-108">Members</span></span>
|<span data-ttu-id="44ba1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="44ba1-109">Member</span></span>|<span data-ttu-id="44ba1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="44ba1-110">Value</span></span>|<span data-ttu-id="44ba1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ba1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ba1-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="44ba1-112">none</span></span>|<span data-ttu-id="44ba1-113">,0</span><span class="sxs-lookup"><span data-stu-id="44ba1-113">0</span></span>|<span data-ttu-id="44ba1-114">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="44ba1-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="44ba1-115">certificado</span><span class="sxs-lookup"><span data-stu-id="44ba1-115">certificate</span></span>|<span data-ttu-id="44ba1-116">1</span><span class="sxs-lookup"><span data-stu-id="44ba1-116">1</span></span>|<span data-ttu-id="44ba1-117">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="44ba1-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="44ba1-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="44ba1-118">derivedCredential</span></span>|<span data-ttu-id="44ba1-119">duas</span><span class="sxs-lookup"><span data-stu-id="44ba1-119">2</span></span>|<span data-ttu-id="44ba1-120">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="44ba1-120">Use a derived credential for certificate source.</span></span>|



