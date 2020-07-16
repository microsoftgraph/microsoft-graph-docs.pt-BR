---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d0e462ab93b60796e8cbb4463c19799ba9033cd2
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038643"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Confira os destaques das novidades do Microsoft Graph e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista completa das atualizações da API, consulte as seções [May](changelog.md#may-2020) [e o](changelog.md#june-2020) que são as do changelog da API. 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="july-2020-new-and-generally-available"></a>Julho de 2020: novo e geralmente disponível

### <a name="change-notifications"></a>Notificações de alteração
Removido o erronously introduziu a propriedade **sequenceNumber** do recurso [changeNotification](/graph/api/resources/changenotification) .

## <a name="july-2020-new-in-preview-only"></a>Julho de 2020: novo na visualização apenas

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
Use as permissões de aplicativo `Printer.ReadWrite.All` e a [codificação IPP (Internet Printing Protocol)](https://tools.ietf.org/html/rfc8010) para [atualizar uma impressora](/graph/api/printer-update?view=graph-rest-beta).

## <a name="june-2020-new-and-generally-available"></a>Junho de 2020: novo e geralmente disponível

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
- Use o `Accept-Language` cabeçalho HTTP ao [criar uma reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) para fornecer informações de ingresso com base na localidade.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) para retornar uma reunião online que tenha um valor **externalId** especificado ou crie um se nenhum já existir, para simplificar a incorporação da reunião resultante em um calendário de terceiros.

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:
  - Use a propriedade **pendingOperations** para identificar quaisquer [operações](/graph/api/resources/pendingoperations) que possam atualizar o conteúdo binário de um arquivo do [driveItem](/graph/api/resources/driveitem) , que estão aguardando conclusão.
  - [Restaure](/graph/api/driveitem-restore) um **driveItem** que tenha sido excluído e esteja na lixeira no onedrive Personal.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo). A configuração é compatível com o OneDrive Personal.
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos [dados](/graph/api/resources/file) do arquivo.
- Use o `deferCommit` parâmetro para adiar a criação final ao [carregar normalmente um arquivo grande](/graph/api/driveitem-createuploadsession) para o onedrive for Business, até que um aplicativo faça uma solicitação para concluir o carregamento.
- Use a propriedade **fileSize** para fornecer como parte do parâmetro de **Item** uma previsão, para fazer uma verificação de cota antes de [carregar um arquivo](/graph/api/driveitem-createuploadsession) no onedrive Personal.
- Encontre [adicionadostorageplaninformation](/graph/api/resources/storageplaninformation) por meio da propriedade **quota** de um recurso [drive](/graph/api/resources/drive) para ver se há mais planos de cota de armazenamento disponíveis.

### <a name="groups"></a>Grupos
Use permissões de aplicativo `Group.Read.All` e `Group.ReadWrite.All` para obter recursos de [conversa](/graph/api/resources/conversation) de grupo e [thread de conversa](/graph/api/resources/conversationthread) .

### <a name="identity-and-access"></a>Identidade e acesso 
- GA de dois conjuntos de APIs para [proteção de identidade](/graph/api/resources/identityprotectionroot): [detecção de risco](/graph/api/resources/riskdetection) e APIs de [usuário arriscadas](/graph/api/resources/riskyuser) .

### <a name="security"></a>Segurança
- Acompanhar o seguinte como propriedades de um [alerta](/graph/api/resources/alert?view=graph-rest-1.0):
  - IDs de incidentes relacionados ao alerta.
  - Identifique um [recurso](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) como atacado ou como um recurso relacionado no alerta.
  - Especifique os locais de origem e de destino de uma [conexão de rede](/graph/api/resources/networkconnection?view=graph-rest-1.0) relacionada ao alerta.

### <a name="sites-and-lists"></a>Sites e listas
Especifique dados de localização geográfica em uma [definição de coluna](/graph/api/resources/columndefinition) para um recurso de [lista](/graph/api/resources/list) do SharePoint.

### <a name="teamwork"></a>Teamwork
- Use a permissão delegada [AppCatalog. Read. All](/graph/permissions-reference#appcatalog-resource-permissions) para listar [aplicativos](/graph/api/resources/teamsapp?view=graph-rest-1.0) do catálogo de aplicativos do Microsoft Teams.
- [Obtenha informações sobre a pasta](/graph/api/channel-get-filesfolder) que mapeia a guia **arquivos** de um [canal](/graph/api/resources/channel)do teams.
- [Obtenha o canal padrão](/graph/api/team-get-primarychannel), rotulado como **geral**, de uma [equipe](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Junho de 2020: novo na visualização apenas

### <a name="calendar"></a>Calendário
Além de controlar as alterações incrementais em eventos em um **calendarView** (coleção ou eventos delimitados pelas datas de início _e_ término), use a função [Delta](/graph/api/event-delta?view=graph-rest-beta) em eventos em uma caixa de correio de usuário ou eventos em um calendário de usuário específico.

### <a name="cloud-communications--presence"></a>Comunicações em nuvem | Presença
[Obter o status de presença](/graph/api/presence-get?view=graph-rest-beta) de todos os usuários em uma organização ou de um usuário específico na organização. grgr

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Especifique as [margens de impressão](/graph/api/resources/printmargin?view=graph-rest-beta) ao configurar um [documento para impressão](/graph/api/resources/printdocument?view=graph-rest-beta).
- Suporte para os seguintes [recursos de impressora](/graph/api/resources/printercapabilities?view=graph-rest-beta):
  - direções de feed
  - imprimir intervalos de páginas
  - resolução de impressão em DPI
  - tamanho máximo da fila de trabalhos de impressão em bytes
  - bandejas de entrada
  - margens
  - Agrupamento
  - escala de documentos
- Suporte para resolução de impressão (DPI) e escala de documentos como parte das [configurações de impressora padrão](/graph/api/resources/printerdefaults?view=graph-rest-beta).
- Suporte para as seguintes definições de [configuração de documento](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta) :
  - bandejas de entrada
  - bandejas de saída
  - tamanhos de mídia
  - margens
  - tipos de mídia
  - acabamentos como grampeamento ou associação
  - páginas por folha
  - layout de várias páginas que especifica a direção para o layout de páginas por folha
  - Agrupamento
  - ajuste
- Expanda documentos ao [listar os trabalhos do pring](/graph/api/printer-list-jobs?view=graph-rest-beta).
- [Registre uma impressora]() e use o recurso [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta) para rastrear e verificar o registro da impressora.
- [Obter operação de registro da impressora de longa duração](/graph/api/printoperation-get?view=graph-rest-beta) no usuário atual ou no locatário do aplicativo.
- Algumas renomeação de propriedades e tipos de enumeração-veja detalhes nas atualizações de [junho](changelog.md#june-2020) de changelog para impressão em nuvem.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [junho](changelog.md#june-2020) no beta.

### <a name="education"></a>Educação
- Pode usar permissões delegadas `EduRoster.ReadBasic` para [obter](/graph/api/educationuser-get?view=graph-rest-beta) a ID de um [professor](/graph/api/resources/educationteacher?view=graph-rest-beta) ou [aluno](/graph/api/resources/educationstudent?view=graph-rest-beta) em um programa de origem externo, como a propriedade **externalId** .
- Use a propriedade **ExternalSource** para controlar o valor `lms` se uma organização ou uma [organização](/graph/api/resources/educationorganization?view=graph-rest-beta) de educação for criada a partir de um sistema de gerenciamento de aprendizado (LMS). [class](/graph/api/resources/educationclass?view=graph-rest-beta)

### <a name="identity-and-access"></a>Identidade e acesso
- Os profissionais de ti podem usar os recursos de [conectores](/graph/api/resources/connector?view=graph-rest-beta) que são agentes leves para se conectarem ao [proxy de aplicativo do Azure ad](/azure/active-directory/manage-apps/what-is-application-proxy)e [publicar aplicativos Web no local externamente](/graph/api/resources/onpremisespublishing?view=graph-rest-beta), para que os usuários remotos de suas organizações possam acessar esses aplicativos de uma maneira segura.
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) em nível de locatário para habilitar ou desabilitar [a inscrição de autoatendimento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) de usuários externos.
- [Provisione uma conta de usuário sob demanda](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta)e especifique os objetos para provisionar e sincronizar regras a serem executadas.

### <a name="search"></a>Search
- Use aprimoramentos em uma [Propriedade](/graph/api/resources/property?view=graph-rest-beta) de um [esquema](/graph/api/resources/schema?view=graph-rest-beta): **isRefinable** para habilitar a filtragem de resultados de pesquisa e para um controle mais refinado da experiência de pesquisa e **aliases** e **Rótulos** para maior relevância.
- Ser capaz de especificar até 128 recursos de **Propriedade** em um **esquema**.
- Use [Get externalItem](/graph/api/externalitem-get?view=graph-rest-beta) para fins de diagnóstico.

### <a name="users"></a>Usuários
- Use a propriedade **userpurpose** de [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) para identificar e diferenciar uma caixa de correio de um único usuário de uma caixa de correio compartilhada e caixa de correio de equipamento no Exchange Online. 
- Use [as configurações do usuário](/graph/api/resources/usersettings?view=graph-rest-beta) para [obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta) ou [Atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta) [languaes preferenciais e configurações regionais](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta).
- Configurações de usuário é uma relação acessível por meio do [usuário](/graph/api/resources/user?view=graph-rest-beta) que permite uma experiência de usuário consistente entre aplicativos, tocando no perfil de usuário do Azure ad para refletir as mesmas preferências do usuário. Veja [como as configurações de usuário diferenciam as configurações de caixa de correio](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa de desenvolvedores do microsoft 365](https://developer.microsoft.com/office/dev-program), obtenha uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).

