---
title: Termos e condições da empresa no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que definem termos e condições para uma organização de locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 439fd1b4a59a196057210aafd56d9a938573cc45
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723955"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="fd36d-103">Termos e condições da empresa no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fd36d-103">Company terms and conditions in Microsoft Intune</span></span>

<span data-ttu-id="fd36d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd36d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd36d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd36d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd36d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd36d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd36d-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd36d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd36d-108">É possível implantar termos e condições do Intune em grupos de usuários para explicar como o registro, o acesso a recursos de trabalho e o aplicativo Portal da Empresa afetam dispositivos e usuários.</span><span class="sxs-lookup"><span data-stu-id="fd36d-108">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="fd36d-109">Os usuários devem aceitar os termos e condições antes de usarem o Portal da Empresa para registrar e acessar o trabalho deles.</span><span class="sxs-lookup"><span data-stu-id="fd36d-109">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="fd36d-110">É possível criar e implantar várias políticas que contenham diferentes termos e condições.</span><span class="sxs-lookup"><span data-stu-id="fd36d-110">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="fd36d-111">Você também pode produzir versões dos mesmos termos e condições em diferentes idiomas e implantar para os grupos apropriados.</span><span class="sxs-lookup"><span data-stu-id="fd36d-111">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="fd36d-112">Os seguintes recursos do Graph estão disponíveis para gerenciar termos e condições no Intune:</span><span class="sxs-lookup"><span data-stu-id="fd36d-112">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="fd36d-113">Termos e condições</span><span class="sxs-lookup"><span data-stu-id="fd36d-113">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="fd36d-114">Status de aceitação dos termos e das condições</span><span class="sxs-lookup"><span data-stu-id="fd36d-114">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="fd36d-115">Atribuição de termos e condições</span><span class="sxs-lookup"><span data-stu-id="fd36d-115">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="fd36d-116">Atribuição de grupo dos termos e das condições</span><span class="sxs-lookup"><span data-stu-id="fd36d-116">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)