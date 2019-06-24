---
title: Visão geral da API de dispositivos e aplicativos do Intune
description: 'O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização. Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas. '
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: a18096f53dfa88bd37b0cad11639c3b2285206e6
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133765"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="aae01-104">Visão geral da API de dispositivos e aplicativos do Intune</span><span class="sxs-lookup"><span data-stu-id="aae01-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="aae01-105">O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização.</span><span class="sxs-lookup"><span data-stu-id="aae01-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="aae01-106">Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas.</span><span class="sxs-lookup"><span data-stu-id="aae01-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="aae01-107">Se você for um ISV, também poderá usar a API do Intune para gerenciar locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="aae01-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a><span data-ttu-id="aae01-108">Por que se integrar com o Intune?</span><span class="sxs-lookup"><span data-stu-id="aae01-108">Why integrate with Intune?</span></span>

<span data-ttu-id="aae01-109">Você pode usar a API do Intune no Microsoft Graph para acessar informações de dispositivos e aplicativos do Intune, gerenciar dispositivos, gerenciar aplicativos e automatizar o Intune.</span><span class="sxs-lookup"><span data-stu-id="aae01-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="aae01-110">Gerenciar dispositivos</span><span class="sxs-lookup"><span data-stu-id="aae01-110">Manage devices</span></span>

<span data-ttu-id="aae01-111">Você pode usar a API do Intune para:</span><span class="sxs-lookup"><span data-stu-id="aae01-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="aae01-112">Definir e impor políticas de [conformidade de dispositivos](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0), como a complexidade e a duração de senhas, a criptografia, os níveis de proteção de ameaças e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="aae01-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="aae01-113">(As políticas permitidas variam de acordo com o sistema operacional e a versão).</span><span class="sxs-lookup"><span data-stu-id="aae01-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="aae01-114">[Proteger os dados da empresa](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), independentemente de a plataforma do dispositivo ser Windows, Android, Mac ou iOS.</span><span class="sxs-lookup"><span data-stu-id="aae01-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="aae01-115">Criar e implantar políticas de [configuração de dispositivo](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), incluindo o controle de versão/plataforma do sistema operacional, a associação a domínios e o gerenciamento de configurações.</span><span class="sxs-lookup"><span data-stu-id="aae01-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="aae01-116">Criar e implantar políticas de [controle de acesso](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) de dispositivo, incluído, downloads restritos, acesso a acessórios de rede e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="aae01-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="aae01-117">Realizar [ações remotas](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), como localizar o dispositivo, alterar a senha e apagar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aae01-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="aae01-118">Gerenciar aplicativos</span><span class="sxs-lookup"><span data-stu-id="aae01-118">Manage apps</span></span> 

<span data-ttu-id="aae01-119">Você pode usar a API do Intune para executar as seguintes tarefas de gerenciamento de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="aae01-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="aae01-120">Implantar [aplicativos em dispositivos](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) ou impedir que aplicativos sejam implantados.</span><span class="sxs-lookup"><span data-stu-id="aae01-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="aae01-121">Gerenciar o acesso a [livros eletrônicos](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) e serviços relacionados.</span><span class="sxs-lookup"><span data-stu-id="aae01-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="aae01-122">Definir e implantar configurações de aplicativos, configurações de proteção de aplicativos e políticas de uso de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="aae01-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="aae01-123">Automatizar o Intune</span><span class="sxs-lookup"><span data-stu-id="aae01-123">Automate Intune</span></span>

<span data-ttu-id="aae01-124">Automatize o Intune usando a API do Intune para:</span><span class="sxs-lookup"><span data-stu-id="aae01-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="aae01-125">Definir e atribuir controles de acesso [por função](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="aae01-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="aae01-126">Auditar e reportar conformidade, uso e acesso.</span><span class="sxs-lookup"><span data-stu-id="aae01-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="aae01-127">Gerenciar [despesas de telecomunicações](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="aae01-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="aae01-128">Referência da API</span><span class="sxs-lookup"><span data-stu-id="aae01-128">API reference</span></span>
<span data-ttu-id="aae01-129">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="aae01-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="aae01-130">API do Intune no Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="aae01-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="aae01-131">API do Intune no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="aae01-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="aae01-132">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="aae01-132">Next steps</span></span>

- <span data-ttu-id="aae01-133">[Usar o Azure AD para acessar a API do Intune](https://docs.microsoft.com/intune/intune-graph-apis).</span><span class="sxs-lookup"><span data-stu-id="aae01-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="aae01-134">Veja como realizar tarefas comuns usando os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples).</span><span class="sxs-lookup"><span data-stu-id="aae01-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="aae01-135">Saiba como [usar a API REST do Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="aae01-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="aae01-136">Confira o [log de alterações](changelog.md) para obter informações sobre as novidades na API do Intune.</span><span class="sxs-lookup"><span data-stu-id="aae01-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="aae01-137">Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aae01-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
