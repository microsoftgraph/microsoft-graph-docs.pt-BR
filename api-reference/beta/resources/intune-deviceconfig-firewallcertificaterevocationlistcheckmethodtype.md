---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958408"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="85849-103">tipo de enum firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="85849-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="85849-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="85849-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85849-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="85849-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85849-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="85849-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85849-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="85849-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="85849-108">Membros</span><span class="sxs-lookup"><span data-stu-id="85849-108">Members</span></span>
|<span data-ttu-id="85849-109">Membro</span><span class="sxs-lookup"><span data-stu-id="85849-109">Member</span></span>|<span data-ttu-id="85849-110">Valor</span><span class="sxs-lookup"><span data-stu-id="85849-110">Value</span></span>|<span data-ttu-id="85849-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85849-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85849-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="85849-112">deviceDefault</span></span>|<span data-ttu-id="85849-113">0</span><span class="sxs-lookup"><span data-stu-id="85849-113">0</span></span>|<span data-ttu-id="85849-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="85849-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="85849-115">nenhum</span><span class="sxs-lookup"><span data-stu-id="85849-115">none</span></span>|<span data-ttu-id="85849-116">1</span><span class="sxs-lookup"><span data-stu-id="85849-116">1</span></span>|<span data-ttu-id="85849-117">Não verificar a lista de revogação de certificado</span><span class="sxs-lookup"><span data-stu-id="85849-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="85849-118">tentativa</span><span class="sxs-lookup"><span data-stu-id="85849-118">attempt</span></span>|<span data-ttu-id="85849-119">2</span><span class="sxs-lookup"><span data-stu-id="85849-119">2</span></span>|<span data-ttu-id="85849-120">Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de</span><span class="sxs-lookup"><span data-stu-id="85849-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="85849-121">exigir</span><span class="sxs-lookup"><span data-stu-id="85849-121">require</span></span>|<span data-ttu-id="85849-122">3</span><span class="sxs-lookup"><span data-stu-id="85849-122">3</span></span>|<span data-ttu-id="85849-123">Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado</span><span class="sxs-lookup"><span data-stu-id="85849-123">Require a successful CRL check before allowing a certificate</span></span>|





