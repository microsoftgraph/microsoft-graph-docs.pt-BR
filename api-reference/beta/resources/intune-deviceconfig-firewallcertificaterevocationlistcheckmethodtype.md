---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c9a94dc19064fc01d70bfa1123d20fec414eac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526441"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="69361-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="69361-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="69361-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69361-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69361-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69361-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69361-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="69361-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="69361-108">Membros</span><span class="sxs-lookup"><span data-stu-id="69361-108">Members</span></span>
|<span data-ttu-id="69361-109">Membro</span><span class="sxs-lookup"><span data-stu-id="69361-109">Member</span></span>|<span data-ttu-id="69361-110">Valor</span><span class="sxs-lookup"><span data-stu-id="69361-110">Value</span></span>|<span data-ttu-id="69361-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69361-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="69361-112">deviceDefault</span></span>|<span data-ttu-id="69361-113">,0</span><span class="sxs-lookup"><span data-stu-id="69361-113">0</span></span>|<span data-ttu-id="69361-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="69361-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="69361-115">nenhuma</span><span class="sxs-lookup"><span data-stu-id="69361-115">none</span></span>|<span data-ttu-id="69361-116">1 </span><span class="sxs-lookup"><span data-stu-id="69361-116">1</span></span>|<span data-ttu-id="69361-117">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="69361-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="69361-118">Houve</span><span class="sxs-lookup"><span data-stu-id="69361-118">attempt</span></span>|<span data-ttu-id="69361-119">2 </span><span class="sxs-lookup"><span data-stu-id="69361-119">2</span></span>|<span data-ttu-id="69361-120">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="69361-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="69361-121">precisa</span><span class="sxs-lookup"><span data-stu-id="69361-121">require</span></span>|<span data-ttu-id="69361-122">3 </span><span class="sxs-lookup"><span data-stu-id="69361-122">3</span></span>|<span data-ttu-id="69361-123">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="69361-123">Require a successful CRL check before allowing a certificate</span></span>|



