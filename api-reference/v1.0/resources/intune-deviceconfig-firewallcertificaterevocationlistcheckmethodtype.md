---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1eeda2493b91e63d54a45c89ed0f840288f97f43
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532523"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="15190-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="15190-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="15190-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15190-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15190-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15190-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="15190-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="15190-107">Membros</span><span class="sxs-lookup"><span data-stu-id="15190-107">Members</span></span>
|<span data-ttu-id="15190-108">Membro</span><span class="sxs-lookup"><span data-stu-id="15190-108">Member</span></span>|<span data-ttu-id="15190-109">Valor</span><span class="sxs-lookup"><span data-stu-id="15190-109">Value</span></span>|<span data-ttu-id="15190-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="15190-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15190-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="15190-111">deviceDefault</span></span>|<span data-ttu-id="15190-112">,0</span><span class="sxs-lookup"><span data-stu-id="15190-112">0</span></span>|<span data-ttu-id="15190-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="15190-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="15190-114">nenhuma</span><span class="sxs-lookup"><span data-stu-id="15190-114">none</span></span>|<span data-ttu-id="15190-115">1 </span><span class="sxs-lookup"><span data-stu-id="15190-115">1</span></span>|<span data-ttu-id="15190-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="15190-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="15190-117">Houve</span><span class="sxs-lookup"><span data-stu-id="15190-117">attempt</span></span>|<span data-ttu-id="15190-118">2 </span><span class="sxs-lookup"><span data-stu-id="15190-118">2</span></span>|<span data-ttu-id="15190-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="15190-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="15190-120">precisa</span><span class="sxs-lookup"><span data-stu-id="15190-120">require</span></span>|<span data-ttu-id="15190-121">3 </span><span class="sxs-lookup"><span data-stu-id="15190-121">3</span></span>|<span data-ttu-id="15190-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="15190-122">Require a successful CRL check before allowing a certificate</span></span>|




