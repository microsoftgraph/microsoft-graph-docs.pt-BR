---
title: Como trabalhar com APIs de educação no Microsoft Graph
description: As APIs de educação no Microsoft Graph aprimoram os recursos e os dados do Microsoft 365 com informações relevantes para cenários educacionais, incluindo escolas, estudantes, professores, classes, registradoras e atribuições. Isso facilita a criação de soluções que se integram aos recursos educacionais.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 2da92b666ee125b91bd2a3782e2dba3f213b593a
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909692"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Como trabalhar com APIs de educação no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As APIs de educação no Microsoft Graph aprimoram os recursos e os dados do Microsoft 365 com informações relevantes para cenários educacionais, incluindo escolas, estudantes, professores, classes, registradoras e atribuições. Isso facilita a criação de soluções que se integram aos recursos educacionais.

As APIs de educação incluem recursos de listagem e recursos de atribuições que você pode usar para interagir com os serviços de lista e atribuição no Microsoft Teams. Você pode usar esses recursos para gerenciar uma lista de escolas e automatizar as atribuições de aluno.

## <a name="authorization"></a>Autorização

Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso. Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). O aplicativo também precisará das permissões apropriadas. Para saber mais, confira [Permissões de educação](/graph/permissions-reference#education-permissions).

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola

Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo. Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem. Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.

Para acionar uma caixa de diálogo de consentimento, use a chamada REST a seguir.

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

As APIs de lista permitem extrair dados do locatário do Microsoft 365 do School provisionado com [o Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso a informações sobre escolas, seções, professores, estudantes e listagens. As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo). As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API. Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários. Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.

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
- [Obter todas as aulas](../api/educationroot-list-classes.md)
- [Obter aulas em um escola](../api/educationschool-list-classes.md)
- [Listar aulas para um usuário](../api/educationuser-list-classes.md)
- [Adicionar aulas a uma escola](../api/educationschool-post-classes.md)
- [Obter alunos e professores para uma aula](../api/educationclass-list-members.md)
- [Adicionar membros a uma aula](../api/educationclass-post-members.md)
- [Listar professores para uma aula](../api/educationclass-list-teachers.md)
- [Obter usuários em uma escola](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Atribuições

Você pode usar as APIs de educação relacionadas à atribuição para integrar com as atribuições no Microsoft Teams. O Microsoft Teams no Microsoft 365 for Education é baseado nas mesmas APIs de educação e fornece um caso de uso para o que você pode fazer com as APIs. Seu aplicativo pode usar essas APIs para interagir com as atribuições ao longo do ciclo de vida da atribuição. 

As APIs de atribuição fornecem os seguintes recursos-chave:

- [educationAssignment](educationassignment.md) -o objeto principal da API assignments. Representa uma tarefa ou unidade de trabalho atribuída a um membro de aluno ou de equipe em uma classe como parte de seu estudo.
- [educationSubmission](educationsubmission.md) -representa os recursos que um indivíduo (ou grupo) envia para uma atribuição e a grade associada e o feedback da atribuição.
- [educationResource](educationresource.md) -representa o objeto de aprendizado que está sendo atribuído ou enviado. Um **educationResource** está associado a um **educationAssignment** e/ou um **educationSubmission**.

As APIs de atribuição dão suporte aos seguintes cenários:

- [Criar tarefa](../api/educationclass-post-assignments.md)
- [Publicar tarefa](../api/educationassignment-publish.md)
- [Criar recurso de tarefa](../api/educationassignment-post-resources.md)
- [Criar recurso de envio](../api/educationsubmission-post-resources.md)
- [Enviar atribuição](../api/educationsubmission-submit.md)
- [Não enviar atribuição](../api/educationsubmission-unsubmit.md)
- [Retornar notas e comentários para o estudante](../api/educationsubmission-return.md)
- [Obter detalhes de atribuição](../api/educationuser-list-assignments.md)

A seguir estão alguns casos de uso comuns para as APIs de educação relacionadas à atribuição.

| Caso de uso                    | Descrição                                                                                                         | Confira também                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| Criar atribuições          | Um sistema externo pode criar uma atribuição para a classe e anexar recursos à atribuição.                   | [Criar tarefa](../api/educationassignment-post-resources.md) |
| Ler informações de atribuição | Um aplicativo de análise pode obter informações sobre atribuições e envios de alunos, incluindo datas e notas. | [Obter tarefa](../api/educationassignment-get.md)               |
| Acompanhar envios de alunos   | Seu aplicativo pode fornecer um painel de professores que mostra quantos envios de alunos precisam ser compensados.           | [Recurso de envio](educationsubmission.md)                     |

## <a name="school-data-sync-management"></a>Gerenciamento escolar de sincronização de dados

O [School Data Sync](https://sds.microsoft.com/) ajuda a automatizar o processo de importação e sincronização de dados de lista de sistemas de informações do aluno com o Active Directory do Azure (Azure AD) e o Microsoft 365. Você pode usar as APIs de gerenciamento de sincronização de dados da escola no Microsoft Graph para configurar a sincronização de um arquivo CSV ou de um conector de API SIS suportado.

As APIs de gerenciamento de sincronização de dados da escola oferecem suporte aos seguintes cenários:

- [Listar perfis de sincronização](../api/educationsynchronizationprofile-list.md)
- [Obter perfil de sincronização](../api/educationsynchronizationprofile-get.md)
- [Criar perfil de sincronização](../api/educationsynchronizationprofile-post.md)
- [Excluir perfil de sincronização](../api/educationsynchronizationprofile-delete.md)
- [Pausar uma sincronização contínua](../api/educationsynchronizationprofile-pause.md)
- [Retomar uma sincronização pausada](../api/educationsynchronizationprofile-resume.md)
- [Redefinir uma sincronização](../api/educationsynchronizationprofile-reset.md)
- [Iniciar a sincronização de arquivos carregados](../api/educationsynchronizationprofile-start.md)
- [Obter uma URL de upload](../api/educationsynchronizationprofile-uploadurl.md)
- [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md)
- [Obter erros de sincronização](../api/educationsynchronizationerrors-get.md)

## <a name="whats-new"></a>Novidades

Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

Use as APIs de educação do Microsoft Graph para criar soluções de educação que acessam as listas de alunos e as listagens da escola. Para saber mais:

- Explore os recursos e os métodos mais úteis para seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
