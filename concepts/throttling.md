---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8af7a4ce6c303e2ac07e4387ff3dbad38abd735e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408089"
---
# <a name="microsoft-graph-throttling-guidance"></a>Diretrizes de limitação do Microsoft Graph

Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.

Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>O que acontece quando a limitação ocorre?
<!-- markdownlint-enable MD026 -->

Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.

## <a name="common-throttling-scenarios"></a>Cenários comuns de limitação

As causas mais comuns de limitação dos clientes incluem:

- Um grande número de solicitações em todos os aplicativos em um locatário.
- Um grande número de solicitações de um aplicativo específico entre todos os locatários.

## <a name="best-practices-to-handle-throttling"></a>Práticas recomendadas para lidar com a limitação

Estas são as práticas recomendadas para lidar com a limitação:

- Reduza o número de operações por solicitação.
- Reduza a frequência de chamadas.
- Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.

Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.

1. Aguarde o número de segundos especificado no cabeçalho `Retry-After`.
2. Repita a solicitação.
3. Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.

Atualmente, os seguintes recursos oferecem atualmente um cabeçalho `Retry-After`:

- [Usuário](/graph/api/resources/user?view=graph-rest-1.0)
- [Foto](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [Email](/graph/api/resources/message?view=graph-rest-1.0)
- [Calendário (usuários e grupos)](/graph/api/resources/event?view=graph-rest-1.0)
- [Contato](/graph/api/resources/contact?view=graph-rest-1.0)
- [Anexo](/graph/api/resources/attachment?view=graph-rest-1.0)
- [Conversas em grupo](/graph/api/resources/conversation?view=graph-rest-1.0)
- [Pessoas e social](/graph/api/resources/social-overview?view=graph-rest-beta)
- [Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)
- [Item externo (Pesquisa da Microsoft)](/graph/api/resources/externalitem?view=graph-rest-beta)
- [Relatório](/graph/api/resources/report)
- [Assinatura](/graph/api/resources/subscription)
- [Solicitação de avaliação de ameaças](/graph/api/resources/threatassessmentrequest)
- [Solicitação de avaliação de email](/graph/api/resources/mailassessmentrequest)
- [Solicitação de avaliação de arquivo de email](/graph/api/resources/emailfileassessmentrequest)
- [Solicitação de avaliação de arquivo](/graph/api/resources/fileassessmentrequest)
- [Solicitação de avaliação de URL](/graph/api/resources/urlassessmentrequest)
- [Resultado da avaliação de ameaças](/graph/api/resources/threatassessmentresult)
- [Tendência](/graph/api/resources/insights-trending)
- [Percepção utilizada](/graph/api/resources/insights-used)
- [Percepção compartilhada](/graph/api/resources/insights-shared)
- [Configurações do usuário](/graph/api/resources/usersettings)
- [Convite](/graph/api/resources/invitation)

Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://docs.microsoft.com/azure/architecture/patterns/throttling).

> [!NOTE]
> Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada. Você também pode implementar [padrões mais avançados](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.
>
> Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.

## <a name="best-practices-to-avoid-throttling"></a>Práticas recomendadas para evitar a limitação

Padrões de programação como pesquisando continuamente um recurso para verificar se há atualizações e a verificação regular das coleções de recursos para verificar se há recursos novos ou excluídos, possuem maior propensão de levar aplicativos a serem regulados e prejudicam o desempenho geral. Em vez disso, você deve aproveitar o [controle de alterações](delta-query-overview.md) e [notificações de alteração](webhooks.md) quando estiverem disponíveis.

>[!NOTE]
>[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) descrevem as práticas recomendadas em detalhes.

## <a name="service-specific-limits"></a>Limites específicos do serviço

O Microsoft Graph permite que você acesse os dados em [vários serviços](overview-major-services.md), como o Outlook ou o Azure Active Directory. Esses serviços impõem seus próprios limites de controle que afetam os aplicativos que usam o Microsoft Graph para acessá-los.

Qualquer solicitação poderá ser avaliada em relação a vários limites, dependendo do escopo do limite (por aplicativo em todos os locatários, por locatário para todos os aplicativos, por aplicativo por locatário, e assim por diante), do tipo de solicitação (GET, POST, PATCH e assim por diante) e de outros fatores. O primeiro limite a ser alcançado dispara o comportamento de limitação. Além dos limites de serviço específicos descritos na seção, os seguintes limites globais se aplicam:

| Tipo de solicitação | Por aplicativo em todos os locatários  |
| ------------ | ------------------------ |
| Qualquer          | 2000 solicitações por segundo |

> [!NOTE]
> Os limites específicos descritos aqui estão sujeitos a alterações.

> **Nota:** Nesta seção, o termo *locatário* refere-se à organização Microsoft 365 onde o aplicativo está instalado. Este inquilino pode ser o mesmo onde o aplicativo foi criado, no caso de um único aplicativo de inquilino, ou pode ser diferente, no caso de [um aplicativo de vários inquilinos](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Limites de serviço do Outlook

Os limites de serviço do Outlook são avaliados para cada combinação de ID de aplicativo e caixa de correio. Em outras palavras, os limites descritos se aplicam a um aplicativo específico ao acessar uma caixa de correio específica (usuário ou grupo). Se um aplicativo exceder o limite de uma caixa de correio, isso não afetará a capacidade de acessar outra caixa de correio. Os seguintes limites se aplicam à nuvem pública, bem como às [ implementações de nuvens nacionais](/graph/deployments).

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | v1.0 e pontos finais beta   |
| 15 megabytes (MB) de upload (PATCH, POST, PUT) em um período de 30 segundos | v1.0 e pontos finais beta   |

#### <a name="outlook-service-resources"></a>Recursos de serviço do Outlook

Os recursos a seguir são fornecidos pelo serviço do Outlook.

##### <a name="calendar-api-resources"></a>Recursos da API do calendário

- [event](/graph/api/resources/event)
- [eventMessage](/graph/api/resources/eventmessage)
- [calendar](/graph/api/resources/calendar)
- [calendarGroup](/graph/api/resources/calendargroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)
- [place (preview)](/graph/api/resources/place)

##### <a name="mail-api-resources"></a>Recursos da API do email

- [message](/graph/api/resources/message)
- [mailFolder](/graph/api/resources/mailfolder)
- [mailSearchFolder](/graph/api/resources/mailsearchfolder)
- [messageRule](/graph/api/resources/messagerule)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a>Recursos da API de contatos pessoais

- [contato](/graph/api/resources/contact)
- [contactFolder](/graph/api/resources/contactfolder)
- [outlookCategory](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a>Recursos da inteligência social e do local de trabalho 

- [person](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a>Recursos da API de tarefas pendentes (visualização)

- [outlookTask](/graph/api/resources/outlooktask)
- [outlookTaskFolder](/graph/api/resources/outlooktaskfolder)
- [outlookTaskGroup](/graph/api/resources/outlooktaskgroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a>Limites dos serviços de comunicação em nuvem

| Recurso      | Limites por aplicativo e por inquilino    |
| -------------- | ------------ |
| [Chamadas](/graph/api/resources/call) | 10.000 chamadas/mês e 100 chamadas simultâneas   |
| [Informações sobre a reunião ](/graph/api/resources/meetinginfo)   | 2000 reuniões/usuário a cada mês |
| [Presença](/graph/api/resources/presence) (pré-visualização)   | 2 rps |

### <a name="onenote-service-limits"></a>Limites do serviço OneNote

| Tipo de limite | Limitar por aplicativo por usuário (contexto delegado) | Limite por aplicativo (contexto somente de aplicativo) |
| ------------ | ------- | ------- |
| Taxa de solicitações | 120 solicitações por 1 minuto e 400 por 1 hora | 240 solicitações por 1 minuto e 800 por 1 hora |
| Solicitações simultâneas | 5 solicitações simultâneas | 20 solicitações simultâneas |

Os limites anteriores se aplicam aos seguintes recursos:  
onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation

Você pode encontrar informações adicionais sobre as práticas recomendadas no [limitação da API do OneNote e como evitá-la](https://developer.microsoft.com/pt-BR/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).  

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="project-rome-service-limits"></a>Limites de serviços do Project Rome

| Tipo de solicitação | Limitar por usuário a todos os aplicativos |
| ------------ | --------------------------- |
| OBTER          | 400 solicitações a cada 5 minutos e 12000 solicitações por dia |
| POSTAR, COLOCAR, CORRIGIR, EXCLUIR | 100 solicitações a cada 5 minutos e 8000 solicitações por dia |

Os limites anteriores se aplicam aos seguintes recursos:  
activityHistoryItem, userActivity

### <a name="microsoft-teams-service-limits"></a>Limites do serviço do Microsoft Teams

Os limites são expressos como solicitações por segundo (rps).

| Tipo de solicitação do Teams                                   | Limitar por aplicativo por locatário        | Limitar por aplicativo em todos os locatários      |
|------------------------------------------------------|---------------------------------|------------|
| Todas as chamadas de API do Graph para o Microsoft Teams              | 15000 solicitações a cada 10 segundos | n/d |
| OBTER equipe, canal, guia, installedApps, appCatalogs   | 60 rps                          | 600 rps |
| Canal POST/PUT, guia, installedApps, appCatalogs    |  30 rps                         | 300 rps  |
| PATCH da equipe, canal, guia, installedApps, appCatalogs |  30 rps                         | 300 rps  |
| EXCLUIR canal, Tab, installedApps, appCatalogs      |  15 rps                         | 150 rps  |
| OBTER /teams/```{team-id}```, joinedTeams              |  30 rps                         | 300 rps  |
| POSTAR /teams/```{team-id}```, COLOCAR /groups/```{team-id}```/team, clone | 6 rps | 150 rps  | 
| OBTER mensagem do canal  | 5 rps | 100 rps |
| OBTER 1:1/mensagem de chat do grupo  | 3 rps | 30 rps |
| POSTAR mensagem do canal | 2 rps | 20 rps |
| POSTAR 1:1/mensagem de chat do grupo | 2 rps | 20 rps |
| OBTENHA /equipes/```{team-id}```/programação e todas as APIs neste caminho | 60 rps | 600 rps |
| PUBLIQUE, CORRIJA, COLOQUE /equipes/```{team-id}```/ programação e todas as APIs neste caminho | 30 rps | 300 rps |
| APAGAR /equipe/```{team-id}```/programação e todas as APIs neste caminho | 15 rps | 150 rps |

É possível emitir, no máximo, 4 solicitações por segundo por aplicativo em uma determinada equipe ou canal.
Um máximo 3.000 mensagens por aplicativo por dia podem ser enviadas para um determinado canal.

Confira também [limites do Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) e [requisitos de votação](/graph/api/resources/teams-api-overview#polling-requirements).

### <a name="information-protection"></a>Proteção de informações

Os seguintes limites se aplicam a qualquer solicitação no `/informationProtection`.

| Operation                 | Limite por inquilino                                            | Limite por recurso (email, URL, arquivo)                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 150 solicitações a cada 15 minutos e 10000 solicitações a cada 24 horas | 1 solicitação a cada 15 minutos e 3 solicitações a cada 24 horas |

Os limites anteriores se aplicam aos seguintes recursos:  
threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.

### <a name="identity-protection-and-conditional-access-service-limits"></a>Proteção da identidade e limites do serviço de acesso condicional

| Tipo de solicitação | Limitar por locatário para todos os aplicativos |
| ------------ | ------- |
| Qualquer | 1 solicitação por segundo |

Os limites anteriores aplicam-se aos seguintes recursos:  
Detecçãoderisco, Usuárioderisco, HistóricodeItemdeUsuárioderisco, NomedoLocal, paísNomedoLocal, ipNomedoLocal, PolíticadeAcessoCondicional.

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` em respostas `429 Too Many Requests`.

### <a name="insights-service-limits"></a>Percepção dos limites de serviço

Os seguintes limites se aplicam a qualquer pedido em `me/insights` ou `users/{id}/insights`.

| Limite                                                      | Aplicável a      |
|------------------------------------------------------------|-----------------|
| 10.000 solicitações de API em um período de 10 minutos                  | pontos de extremidade v1.0 e beta |
| 4 solicitações simultâneas                                      | v1.0 e pontos finais beta   |

### <a name="microsoft-graph-reports-service-limits"></a>Limites do serviço de relatórios do Microsoft Graph

Os seguintes limites se aplicam a qualquer solicitação no `/reports`.

| Operation                 | Limitar por aplicativo por locatário     | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|----------------------------|
| Qualquer pedido (CSV)         | 14 solicitações a cada 10 minutos   | 40 solicitações a cada 10 minutos |
| Qualquer solicitação (JSON, beta)  | 100 solicitações a cada 10 minutos  | n/d                        |

Os limites anteriores aplicam-se individualmente a cada relatório de API. Por exemplo, uma solicitação de relatório da API do usuário da Microsoft Teams e uma solicitação de relatório da API do usuário do Outlook dentro de 10 minutos contará como 1 solicitação de 14 para cada API e não 2 solicitações de 14 para ambas.

### <a name="invitation-manager-service-limits"></a>Limites de serviço do gerenciador de convite

Os seguintes limites se aplicam a qualquer solicitação no `/invitations`.

| Operation                 | Limitar por locatário para todos os aplicativos |
|---------------------------|------------------------------|
| Qualquer operação             | 150 solicitações a cada 5 segundos   |

### <a name="security-detections-and-incidents-service-limits"></a>Limites de serviços de detecção de segurança e incidentes

Os seguintes limites se aplicam a qualquer solicitação no `/security`.

| Operation                  | Limitar por aplicativo por locatário     |
|----------------------------|------------------------------|
| Qualquer operação em `alert`, `securityActions`,  `secureScore` | 150 solicitações por minuto      |
| Qualquer operação em `tiIndicator` | 1000 solicitações por minuto |
| Qualquer operação em `secureScore` ou `secureScorecontrolProfile` | 10.000 solicitações de API em um período de 10 minutos |
| Qualquer operação em `secureScore` ou `secureScorecontrolProfile` | 4 solicitações simultâneas |

### <a name="open-and-schema-extensions-service-limits"></a>Limitações de serviços à extensões de esquema e abertas

| Tipo de solicitação | Limitar por aplicativo por locatário |
| ------------ | ------------------------ |
| Qualquer          | 455 solicitações a cada 10 segundos |

Os limites acima se aplicam aos seguintes recursos: openTypeExtension, schemaExtension, administrativeUnit, contato, dispositivo, evento, grupo, mensagem, organização, postagem e usuário.

### <a name="files-and-lists-service-limits"></a>Limites de serviço dos arquivos e listas

Os limites de serviço do OneDrive, OneDrive for Business e SharePoint Online não estão disponíveis. Para mais informações, confira [Por que não é possível saber o limites exatos?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

As informações anteriores aplicam-se aos seguintes recursos:  
baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, List, listItem, listItemVersion, permission, sharedDriveItem, site e thumbnailSet.

### <a name="tasks-and-plans-service-limits"></a>Limites de serviços de tarefas e planos

Os limites de serviço do Planner não estão disponíveis.

As informações anteriores aplicam-se aos seguintes recursos:  
planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, e plannerUser.

### <a name="identity-and-access-data-policy-operation-service-limits"></a>Limites de operação de serviços de política de dados de identidade e acesso

| Tipo de solicitação | Limite por inquilino |
| ------------ | ---------------- |
| Postar no `exportPersonalData` | 1.000 solicitações por dia para todos os assuntos e 100 por assunto por dia |
| Qualquer outra solicitação | 10.000 solicitações por minuto |

Os limites anteriores se aplicam aos seguintes recursos: dataPolicyOperation.

> **Observação:** os recursos listados acima não retornam um cabeçalho `Retry-After` nas respostas `429 Too Many Requests`.

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>Limites do serviço de Educação

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Limites de serviço do Excel

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a>Limites do serviço de registros de auditoria de identidade e acesso

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a>Limites de serviço dos fornecedores de identidade

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Limites de serviço Intune

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a>Limites do serviço Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Limites do serviço de assinatura

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
