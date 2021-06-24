---
title: Registrar dispositivos corporativos usando o Intune - API Graph Microsoft
description: Lista a API Graph microsoft para pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatários.
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daefbf23d8aa70cdd3f81fdcb4afb69dd2590ba7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108933"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="83dad-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="83dad-103">Enroll corporate-owned devices by using Intune</span></span>

<span data-ttu-id="83dad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83dad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83dad-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83dad-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83dad-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83dad-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83dad-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83dad-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83dad-108">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="83dad-108">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="83dad-109">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="83dad-109">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="83dad-110">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="83dad-110">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="83dad-111">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="83dad-111">Device management</span></span>](intune-enrollment-devicemanagement.md)
- [<span data-ttu-id="83dad-112">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="83dad-112">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="83dad-113">Identidade importada do dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="83dad-113">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="83dad-114">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="83dad-114">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="83dad-115">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="83dad-115">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="83dad-116">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="83dad-116">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="83dad-117">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="83dad-117">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)