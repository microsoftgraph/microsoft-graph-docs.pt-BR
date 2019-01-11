---
title: Como trabalhar com APIs de educação no Microsoft Graph
description: A formação APIs no Microsoft Graph melhore os recursos do Office 365 e os dados com as informações relevantes para cenários de educação, incluindo escolas, alunos, professores, classes, inscrições e atribuições. Isso facilita a criação de soluções que se integram aos recursos educacionais.
localization_priority: Normal
ms.openlocfilehash: 3f04ee2817a7346710608df0e97a89251103acc9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852469"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Como trabalhar com APIs de educação no Microsoft Graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

A formação APIs no Microsoft Graph melhore os recursos do Office 365 e os dados com as informações relevantes para cenários de educação, incluindo escolas, alunos, professores, classes, inscrições e atribuições. Isso facilita a criação de soluções que se integram aos recursos educacionais.

A formação APIs incluem recursos de rostering e recursos de atribuições que você pode usar para interagir com os serviços de rostering e a atribuição no Microsoft Teams. Você pode usar estes recursos para gerenciar uma lista de participação da escola e automatizar atribuições do estudante.

## <a name="authorization"></a>Autorização

Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso. Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). O aplicativo também precisará das permissões apropriadas. Para saber mais, confira [Permissões de educação](/graph/permissions-reference#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola 

Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo. Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem. Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.

Para acionar uma caixa de diálogo de consentimento, use a chamada REST a seguir.

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|Parâmetro|Descrição|
|:--------|:----------|
|Tenant|ID do locatário da escola. Use a ID completa, que inclui onmicrosoft.com.|
|clientId|ID do cliente do aplicativo.|
|redirectUrl|URL de redirecionamento do aplicativo.|


## <a name="rostering"></a>Lista de participantes

As APIs de lista de participantes permitem extrair dados do locatário do Office 365 de uma escola provisionado com o [Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso às informações sobre escolas, seções, professores, alunos e listas de participantes. As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo). As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API. Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários. Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.

Você pode usar as APIs de escalação para permitir que um usuário do aplicativo saiba:

- Quem eu sou
- Quais aulas eu frequento ou ministro
- O que preciso fazer e quando

As APIs de escalação fornecem os seguintes recursos-chave:

- [educationSchool](educationschool.md) – representa a escola.
- [educationClass](educationclass.md) – representa uma aula em uma escola.
- [educationTerm](educationterm.md) – representa uma parte designada do ano acadêmico.
- [educationTeacher](educationteacher.md) – representa um usuário com a função principal de ‘Professor’.
- [educationStudent](educationstudent.md) – representa um usuário com a função principal de 'aluno'.

As APIs de escalação dão suporte aos seguintes cenários:

- [Listar todas as escolas](../api/educationroot-list-schools.md) 
- [Listar escolas nas quais uma aula é ministrada](../api/educationclass-list-schools.md)
- [Listar escolas para um usuário](../api/educationuser-list-schools.md)
- [Obter todas as aulas](../api/educationroot_list_classes.md )
- [Obter aulas em um escola](../api/educationschool-list-classes.md)
- [Listar aulas para um usuário](../api/educationuser-list-classes.md)
- [Adicionar aulas a uma escola](../api/educationschool-post-classes.md)
- [Obter alunos e professores para uma aula](../api/educationclass-list-members.md)
- [Adicionar membros a uma aula](../api/educationclass-post-members.md) 
- [Listar professores para uma aula](../api/educationclass-list-teachers.md)
- [Obter usuários em uma escola](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Assignments 

Você pode usar a APIs de educação relacionados a atribuição de integrar com atribuições em Teams da Microsoft. Microsoft Teams no Office 365 para educação se baseia na mesma formação APIs e fornece um caso de uso para que você pode fazer com as APIs. Seu aplicativo pode usar essas APIs para interagir com atribuições em todo o ciclo de vida de atribuição. 

A atribuição APIs oferecem os seguintes recursos principais:

- [educationAssignment](educationassignment.md) - o objeto de núcleo das atribuições API. Representa uma tarefa ou a unidade de trabalho atribuído a um estudante ou membro da equipe em uma classe como parte de sua estudo.
- [educationSubmission](educationsubmission.md) - representa os recursos que um individual (ou de grupo) envia para uma atribuição e o nível associado e comentários para essa atribuição.
- [educationResource](educationresource.md) - representa o aprendizado do objeto ou seja sendo atribuída ou enviados. Um **educationResource** é associado um **educationAssignment** e/ou em um **educationSubmission**.

A atribuição de APIs suportar os seguintes cenários:

- [Criar atribuição](../api/educationclass-post-assignments.md)
- [Publicar atribuição](../api/educationassignment-publish.md)
- [Criar o recurso de atribuição](../api/educationassignment-post-resources.md)
- [Criar o recurso de envio](../api/educationsubmission-post-resources.md)
- [Enviar atribuição](../api/educationsubmission-submit.md) 
- [Atribuição de unsubmit](../api/educationsubmission-unsubmit.md)   
- [Notas de retorno e comentários ao estudante](../api/educationsubmission-return.md) 
- [Conheça os detalhes de atribuição](../api/educationuser-list-assignments.md)

Estes são alguns casos de uso comuns para os APIs de educação relacionados a atribuição.

|Caso de uso|Descrição|Confira também|
|:-------|:----------|:-------|
|Criar atribuições|Um sistema externo pode criar uma atribuição para a classe e anexar recursos à atribuição.|[Criar atribuição](../api/educationassignment-post-resources.md)|
|Leia as informações de atribuição|Um aplicativo de análise pode obter informações sobre atribuições e envios de student, incluindo datas e notas.|[Fazer a atribuição](../api/educationassignment-get.md)|
|Rastrear envios de student|Seu aplicativo pode fornecer um painel de professor que mostra quantos envios de alunos precisam ser graduadas.|[Recurso de envio](educationsubmission.md)|

## <a name="school-data-sync-management"></a>Gerenciamento de sincronização de dados de escola

[Sincronização de dados da escola](https://sds.microsoft.com/) ajuda a automatizar o processo de importação e a sincronização de dados de lista de participação de sistemas de informação de student com o Azure Active Directory (AD Azure) e Office 365. Você pode usar o gerenciamento de sincronização de dados escola APIs no Microsoft Graph para configurar a sincronização de um arquivo CSV ou um conector de API SIS com suporte.

Os dados da escola sincronizar o suporte ao gerenciamento de APIs os seguintes cenários:

- [Perfis de sincronização de lista](../api/educationsynchronizationprofile-list.md)
- [Obtenha o perfil de sincronização](../api/educationsynchronizationprofile-get.md)
- [Criar um perfil de sincronização](../api/educationsynchronizationprofile-post.md)
- [Excluir o perfil de sincronização](../api/educationsynchronizationprofile-delete.md)
- [Pausar uma sincronização em andamento](../api/educationsynchronizationprofile-pause.md)
- [Retomar uma sincronização pausada](../api/educationsynchronizationprofile-resume.md)
- [Redefinir uma sincronização](../api/educationsynchronizationprofile-reset.md)
- [Iniciar sincronização para arquivos carregados](../api/educationsynchronizationprofile-start.md) 
- [Obtenha uma URL de carregamento](../api/educationsynchronizationprofile-uploadurl.md)
- [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md)
- [Obtenha os erros de sincronização](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>Próximas etapas
Use a APIs de educação do Microsoft Graph para construir soluções de educação que acessam as atribuições do estudante e escalações escola. Para saber mais:

- Explore os recursos e os métodos mais úteis para seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

