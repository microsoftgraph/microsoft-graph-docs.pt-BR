---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5c3f9d338ae0a5bf047bb0e8a18d7e7fdb94593
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994124"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="b5016-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="b5016-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="b5016-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5016-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5016-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5016-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5016-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5016-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5016-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="b5016-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="b5016-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b5016-108">Members</span></span>
|<span data-ttu-id="b5016-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b5016-109">Member</span></span>|<span data-ttu-id="b5016-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b5016-110">Value</span></span>|<span data-ttu-id="b5016-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5016-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5016-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b5016-112">deviceDefault</span></span>|<span data-ttu-id="b5016-113">,0</span><span class="sxs-lookup"><span data-stu-id="b5016-113">0</span></span>|<span data-ttu-id="b5016-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b5016-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b5016-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b5016-115">none</span></span>|<span data-ttu-id="b5016-116">1 </span><span class="sxs-lookup"><span data-stu-id="b5016-116">1</span></span>|<span data-ttu-id="b5016-117">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="b5016-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="b5016-118">Houve</span><span class="sxs-lookup"><span data-stu-id="b5016-118">attempt</span></span>|<span data-ttu-id="b5016-119">2 </span><span class="sxs-lookup"><span data-stu-id="b5016-119">2</span></span>|<span data-ttu-id="b5016-120">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="b5016-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="b5016-121">precisa</span><span class="sxs-lookup"><span data-stu-id="b5016-121">require</span></span>|<span data-ttu-id="b5016-122">3 </span><span class="sxs-lookup"><span data-stu-id="b5016-122">3</span></span>|<span data-ttu-id="b5016-123">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="b5016-123">Require a successful CRL check before allowing a certificate</span></span>|






