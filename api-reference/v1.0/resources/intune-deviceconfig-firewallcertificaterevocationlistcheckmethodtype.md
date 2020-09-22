---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 969a94ed8a782989aaf9d34c00fe1f4cc82775ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056706"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="682aa-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="682aa-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="682aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="682aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="682aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="682aa-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="682aa-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="682aa-107">Membros</span><span class="sxs-lookup"><span data-stu-id="682aa-107">Members</span></span>
|<span data-ttu-id="682aa-108">Membro</span><span class="sxs-lookup"><span data-stu-id="682aa-108">Member</span></span>|<span data-ttu-id="682aa-109">Valor</span><span class="sxs-lookup"><span data-stu-id="682aa-109">Value</span></span>|<span data-ttu-id="682aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="682aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="682aa-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="682aa-111">deviceDefault</span></span>|<span data-ttu-id="682aa-112">,0</span><span class="sxs-lookup"><span data-stu-id="682aa-112">0</span></span>|<span data-ttu-id="682aa-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="682aa-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="682aa-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="682aa-114">none</span></span>|<span data-ttu-id="682aa-115">1 </span><span class="sxs-lookup"><span data-stu-id="682aa-115">1</span></span>|<span data-ttu-id="682aa-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="682aa-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="682aa-117">Houve</span><span class="sxs-lookup"><span data-stu-id="682aa-117">attempt</span></span>|<span data-ttu-id="682aa-118">2 </span><span class="sxs-lookup"><span data-stu-id="682aa-118">2</span></span>|<span data-ttu-id="682aa-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="682aa-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="682aa-120">precisa</span><span class="sxs-lookup"><span data-stu-id="682aa-120">require</span></span>|<span data-ttu-id="682aa-121">3 </span><span class="sxs-lookup"><span data-stu-id="682aa-121">3</span></span>|<span data-ttu-id="682aa-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="682aa-122">Require a successful CRL check before allowing a certificate</span></span>|









