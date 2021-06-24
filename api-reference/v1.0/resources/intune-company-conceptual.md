---
title: Termos e condições da empresa em Microsoft Intune - API Graph Microsoft
description: Lista os pontos de extremidade Graph API do Microsoft para Intune (REST) que suportam termos e condições da empresa.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0a67f9704e68e75a1875cad16a3fca91e97081fe
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108849"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="a75cf-103">Termos e condições da empresa no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a75cf-103">Company terms and conditions in Microsoft Intune</span></span>

<span data-ttu-id="a75cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a75cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a75cf-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a75cf-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a75cf-106">É possível implantar termos e condições do Intune em grupos de usuários para explicar como o registro, o acesso a recursos de trabalho e o aplicativo Portal da Empresa afetam dispositivos e usuários.</span><span class="sxs-lookup"><span data-stu-id="a75cf-106">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="a75cf-107">Os usuários devem aceitar os termos e condições antes de usarem o Portal da Empresa para registrar e acessar o trabalho deles.</span><span class="sxs-lookup"><span data-stu-id="a75cf-107">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="a75cf-108">É possível criar e implantar várias políticas que contenham diferentes termos e condições.</span><span class="sxs-lookup"><span data-stu-id="a75cf-108">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="a75cf-109">Você também pode produzir versões dos mesmos termos e condições em diferentes idiomas e implantar para os grupos apropriados.</span><span class="sxs-lookup"><span data-stu-id="a75cf-109">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="a75cf-110">Os seguintes recursos do Graph estão disponíveis para gerenciar termos e condições no Intune:</span><span class="sxs-lookup"><span data-stu-id="a75cf-110">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="a75cf-111">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a75cf-111">Device management</span></span>](intune-companyterms-devicemanagement.md)
- [<span data-ttu-id="a75cf-112">Termos e condições</span><span class="sxs-lookup"><span data-stu-id="a75cf-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="a75cf-113">Status de aceitação dos termos e das condições</span><span class="sxs-lookup"><span data-stu-id="a75cf-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="a75cf-114">Atribuição de termos e condições</span><span class="sxs-lookup"><span data-stu-id="a75cf-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)