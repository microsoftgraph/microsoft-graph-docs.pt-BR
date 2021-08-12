---
title: Visão geral da API de dispositivos e aplicativos do Intune
description: 'O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização. Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas. '
author: dougeby
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 373746111008e627dc066024afa9703794e2e95ee99c048f602578b51e7a64a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205182"
---
# <a name="intune-devices-and-apps-api-overview"></a>Visão geral da API de dispositivos e aplicativos do Intune

O Microsoft Intune ajuda as empresas a gerenciar dispositivos e aplicativos em uma organização. Você pode usar a API do Intune no Microsoft Graph para gerenciar dispositivos, aplicativos e até mesmo configurar o Intune enquanto usa suas ferramentas favoritas. 

Se você for um ISV, também poderá usar a API do Intune para gerenciar locatários de clientes.

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a>Por que se integrar com o Intune?

Você pode usar a API do Intune no Microsoft Graph para acessar informações de dispositivos e aplicativos do Intune, gerenciar dispositivos, gerenciar aplicativos e automatizar o Intune.

### <a name="manage-devices"></a>Gerenciar dispositivos

Você pode usar a API do Intune para:

- Definir e impor políticas de [conformidade de dispositivos](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0), como a complexidade e a duração de senhas, a criptografia, os níveis de proteção de ameaças e assim por diante.  (As políticas permitidas variam de acordo com o sistema operacional e a versão).
- [Proteger os dados da empresa](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), independentemente de a plataforma do dispositivo ser Windows, Android, Mac ou iOS.
- Criar e implantar políticas de [configuração de dispositivo](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), incluindo o controle de versão/plataforma do sistema operacional, a associação a domínios e o gerenciamento de configurações.
- Criar e implantar políticas de [controle de acesso](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) de dispositivo, incluído, downloads restritos, acesso a acessórios de rede e transferência de arquivos.
- Realizar [ações remotas](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), como localizar o dispositivo, alterar a senha e apagar o dispositivo.

### <a name="manage-apps"></a>Gerenciar aplicativos 

Você pode usar a API do Intune para executar as seguintes tarefas de gerenciamento de aplicativos:

- Implantar [aplicativos em dispositivos](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) ou impedir que aplicativos sejam implantados.
- Gerenciar o acesso a [livros eletrônicos](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) e serviços relacionados.
- Definir e implantar configurações de aplicativos, configurações de proteção de aplicativos e políticas de uso de aplicativos.

### <a name="automate-intune"></a>Automatizar o Intune

Automatize o Intune usando a API do Intune para:

- Definir e atribuir controles de acesso [por função](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0).
- Auditar e reportar conformidade, uso e acesso.
- Gerenciar [despesas de telecomunicações](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API do Intune no Microsoft Graph v1.0](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [API do Intune no Microsoft Graph beta](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- [Usar o Azure AD para acessar a API do Intune](/intune/intune-graph-apis).
- Veja como realizar tarefas comuns usando os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples).
- Saiba como [usar a API REST do Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).
- Confira o [log de alterações](changelog.md) para obter informações sobre as novidades na API do Intune.
- Explore os [recursos](https://developer.microsoft.com/graph/gallery/) para mais ideias sobre como utilizar o Microsoft Graph.