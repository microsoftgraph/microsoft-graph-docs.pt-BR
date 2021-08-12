---
title: Como trabalhar com APIs de educação no Microsoft Graph
description: As APIs de educação no Microsoft Graph aprimoram os recursos e dados do Microsoft 365 com informações que são relevantes para cenários de educação, incluindo escolas, alunos, professores, aulas e matrículas. Isso facilita a criação de soluções que se integram aos recursos educacionais.
localization_priority: Priority
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: f9d75ee57396aebe2f15518f3d12c675edf7d217fa0609f08af1af6428e12338
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146969"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Como trabalhar com APIs de educação no Microsoft Graph

As APIs de educação no Microsoft Graph aprimoram os recursos e dados do Microsoft 365 com informações que são relevantes para cenários de educação, incluindo escolas, alunos, professores, aulas e matrículas. Isso facilita a criação de soluções que se integram aos recursos educacionais.

As APIs de educação incluem recursos de listagem e recursos de tarefas que você pode usar para interagir com os serviços de listagem no Microsoft Teams. Você pode usar esses recursos para gerenciar uma lista de escolas.

## <a name="authorization"></a>Autorização

Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso. Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](/graph/auth/). O aplicativo também precisará das permissões apropriadas. Para saber mais, confira [Permissões de educação](/graph/permissions-reference#education-permissions).

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola

Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo. Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem. Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.

Para mostrar uma caixa de diálogo de consentimento, use a chamada REST a seguir.

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| Parâmetro   | Descrição                                                               |
| :---------- | :------------------------------------------------------------------------ |
| Tenant      | ID do locatário da escola. Use a ID completa, que inclui onmicrosoft.com. |
| clientId    | ID do cliente do aplicativo.                                                     |
| redirectUrl | URL de redirecionamento do aplicativo.                                                         |

## <a name="rostering"></a>Lista de participantes

As APIs de lista de participantes permitem extrair dados do locatário do Microsoft 365 de uma escola provisionado com o [Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso às informações sobre escolas, seções, professores, alunos e listas de participantes. As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo). As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API. Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários. Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.

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

- [Listar todas as escolas](../api/educationschool-list.md)
- [Listar escolas nas quais uma aula é ministrada](../api/educationclass-list-schools.md)
- [Listar escolas para um usuário](../api/educationuser-list-schools.md)
- [Obter todas as aulas](../api/educationclass-list.md)
- [Obter aulas em um escola](../api/educationschool-list-classes.md)
- [Listar aulas para um usuário](../api/educationuser-list-classes.md)
- [Adicionar aulas a uma escola](../api/educationschool-post-classes.md)
- [Obter alunos e professores para uma aula](../api/educationclass-list-members.md)
- [Adicionar membros a uma aula](../api/educationclass-post-members.md)
- [Listar professores para uma aula](../api/educationclass-list-teachers.md)
- [Obter usuários em uma escola](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Atribuições

Você pode usar as APIs de educação relacionadas a atribuições para integrá-las às atribuições do Microsoft Teams. O Microsoft Teams no Microsoft 365 Educacional é baseado nas mesmas APIs educacionais e fornece um caso de uso para o que você pode fazer com as APIs. Seu aplicativo pode usar essas APIs para interagir com as tarefas em todo o ciclo de vida da tarefa. 

As APIs de atribuição fornecem os seguintes recursos-chave:

- [educationAssignment](educationassignment.md) - O objeto principal da API de atribuições. As atribuições são tarefas ou unidades de trabalho atribuídas a um aluno ou membro da equipe em uma classe como parte do estudo.
- [educationSubmission](educationsubmission.md) - Representa os recursos que um indivíduo (ou grupo) envia para uma tarefa, a nota associada e os comentários para essa tarefa.
- [educationResource](educationresource.md) - Representa o objeto de aprendizagem que está sendo atribuído ou enviado. Um **educationResource** está associado a um **educationAssignment** e/ou um **educationSubmission**.

As APIs de atribuição suportam os seguintes cenários:

- [Criar tarefa](../api/educationclass-post-assignment.md)
- [Publicar tarefa](../api/educationassignment-publish.md)
- [Criar recurso de tarefa](../api/educationassignment-post-resource.md)
- [Criar recurso de envio](../api/educationsubmission-post-resources.md)
- [Enviar tarefa](../api/educationsubmission-submit.md)
- [Cancelar o envio da tarefa](../api/educationsubmission-unsubmit.md)
- [Devolver notas e comentários ao aluno](../api/educationsubmission-return.md)
- [Obter os detalhes da tarefa](../api/educationuser-list-assignments.md)

A seguir estão alguns casos de uso comuns para as APIs educacionais relacionadas a atribuições.

| Caso de uso                    | Descrição                                                                                                         | Veja também                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| Criar tarefas          | Um sistema externo pode criar uma tarefa para a classe e anexar recursos à tarefa.                   | [Criar tarefa](../api/educationassignment-post-resource.md) |
| Leia as informações da atribuição | Um aplicativo de análise pode obter informações sobre tarefas e envios dos alunos, incluindo datas e notas. | [Obter a tarefa](../api/educationassignment-get.md)               |
| Acompanhar os envios dos alunos   | Seu aplicativo pode fornecer um painel do professor que mostra quantos envios de alunos precisam ser avaliados.           | [Recurso de submissão](educationsubmission.md)                     |

## <a name="whats-new"></a>O que há de novo

Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

Use as APIs de educação do Microsoft Graph para construir soluções educacionais que acessam as listas escolares. Para saber mais:

- Explore os recursos e os métodos mais úteis para seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
