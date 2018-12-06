---
title: Visão geral da API de dispositivos e aplicativos do Intune
description: 'O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização. Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas. '
ms.openlocfilehash: fced71d317aa5f2aebfd2c44237ea9087a6be4f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091672"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="fa02c-104">Visão geral da API de dispositivos e aplicativos do Intune</span><span class="sxs-lookup"><span data-stu-id="fa02c-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="fa02c-105">O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização.</span><span class="sxs-lookup"><span data-stu-id="fa02c-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="fa02c-106">Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas.</span><span class="sxs-lookup"><span data-stu-id="fa02c-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="fa02c-107">Se você for um ISV, também poderá usar a API do Intune para gerenciar locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="fa02c-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

## <a name="why-integrate-with-intune"></a><span data-ttu-id="fa02c-108">Por que se integrar com o Intune?</span><span class="sxs-lookup"><span data-stu-id="fa02c-108">Why integrate with Intune?</span></span>

<span data-ttu-id="fa02c-109">Você pode usar a API do Intune no Microsoft Graph para acessar informações de dispositivos e aplicativos do Intune, gerenciar dispositivos, gerenciar aplicativos e automatizar o Intune.</span><span class="sxs-lookup"><span data-stu-id="fa02c-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="fa02c-110">Gerenciar dispositivos</span><span class="sxs-lookup"><span data-stu-id="fa02c-110">Manage devices</span></span>

<span data-ttu-id="fa02c-111">Você pode usar a API do Intune para:</span><span class="sxs-lookup"><span data-stu-id="fa02c-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="fa02c-112">Definir e impor políticas de [conformidade de dispositivos](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0), como a complexidade e a duração de senhas, a criptografia, os níveis de proteção de ameaças e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="fa02c-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="fa02c-113">(As políticas permitidas variam de acordo com o sistema operacional e a versão).</span><span class="sxs-lookup"><span data-stu-id="fa02c-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="fa02c-114">[Proteger os dados da empresa](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), independentemente de a plataforma do dispositivo ser Windows, Android, Mac ou iOS.</span><span class="sxs-lookup"><span data-stu-id="fa02c-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="fa02c-115">Criar e implantar políticas de [configuração de dispositivo](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), incluindo o controle de versão/plataforma do sistema operacional, a associação a domínios e o gerenciamento de configurações.</span><span class="sxs-lookup"><span data-stu-id="fa02c-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="fa02c-116">Criar e implantar políticas de [controle de acesso](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) de dispositivo, incluído, downloads restritos, acesso a acessórios de rede e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="fa02c-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="fa02c-117">Realizar [ações remotas](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), como localizar o dispositivo, alterar a senha e apagar o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fa02c-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="fa02c-118">Gerenciar aplicativos</span><span class="sxs-lookup"><span data-stu-id="fa02c-118">Manage apps</span></span> 

<span data-ttu-id="fa02c-119">Você pode usar a API do Intune para executar as seguintes tarefas de gerenciamento de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="fa02c-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="fa02c-120">Implantar [aplicativos em dispositivos](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) ou impedir que aplicativos sejam implantados.</span><span class="sxs-lookup"><span data-stu-id="fa02c-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="fa02c-121">Gerenciar o acesso a [livros eletrônicos](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) e serviços relacionados.</span><span class="sxs-lookup"><span data-stu-id="fa02c-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="fa02c-122">Definir e implantar configurações de aplicativos, configurações de proteção de aplicativos e políticas de uso de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fa02c-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="fa02c-123">Automatizar o Intune</span><span class="sxs-lookup"><span data-stu-id="fa02c-123">Automate Intune</span></span>

<span data-ttu-id="fa02c-124">Automatize o Intune usando a API do Intune para:</span><span class="sxs-lookup"><span data-stu-id="fa02c-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="fa02c-125">Definir e atribuir controles de acesso [por função](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fa02c-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="fa02c-126">Auditar e reportar conformidade, uso e acesso.</span><span class="sxs-lookup"><span data-stu-id="fa02c-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="fa02c-127">Gerenciar [despesas de telecomunicações](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fa02c-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="fa02c-128">Referência da API</span><span class="sxs-lookup"><span data-stu-id="fa02c-128">API reference</span></span>
<span data-ttu-id="fa02c-129">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="fa02c-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="fa02c-130">API do Intune no Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="fa02c-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="fa02c-131">API do Intune no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="fa02c-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="fa02c-132">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fa02c-132">Next steps</span></span>

- <span data-ttu-id="fa02c-133">[Usar o Azure AD para acessar a API do Intune](https://docs.microsoft.com/intune/intune-graph-apis).</span><span class="sxs-lookup"><span data-stu-id="fa02c-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="fa02c-134">Veja como realizar tarefas comuns usando os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples).</span><span class="sxs-lookup"><span data-stu-id="fa02c-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="fa02c-135">Saiba como [usar a API REST do Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fa02c-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="fa02c-136">Confira o [log de alterações](changelog.md) para obter informações sobre as novidades na API do Intune.</span><span class="sxs-lookup"><span data-stu-id="fa02c-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="fa02c-137">Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fa02c-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
