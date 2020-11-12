---
title: Revisões do Azure AD Access-herdadas
description: Você pode usar as revisões do Azure AD Access para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário. Esta documentação serve para APIs herdadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 9a3b10d4892a2b73e98a92375677745081a9aeed
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000636"
---
# <a name="azure-ad-access-reviews-legacy"></a>Revisões do Azure AD Access (Herdado)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Uma versão mais recente das APIs de revisão do Access pode ser encontrada [aqui](accessreviewsv2-root.md). Essa nova versão só oferece suporte a revisões de associação de grupo no momento. Para revisões de todos os outros recursos, use as APIs herdadas.

Você pode usar as [revisões do Azure ad Access](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário.

Cenários de cliente típicos para revisões de acesso de associações de grupo e acesso de aplicativo são:

- Os clientes podem revisar e certificar o acesso de usuário convidado usando revisões de acesso de seu acesso a aplicativos e associações de grupos. Os revisores podem usar os insights fornecidos para decidir de forma eficiente se os convidados devem ter acesso contínuo.

- Os clientes podem analisar e certificar o acesso do funcionário aos aplicativos e às associações de grupo com as revisões do Access.

- Os clientes podem coletar controles de revisão de acesso em programas que são relevantes para a sua organização para rastrear as revisões de conformidade ou aplicativos sensíveis a riscos.

Há também um recurso relacionado para os clientes revisar e certificar as atribuições de função de usuários administrativos atribuídos às funções do Azure AD, como administrador global ou funções de assinatura do Azure.  Esse recurso está incluído no [Gerenciamento de identidade privilegiado do Azure ad](privilegedidentitymanagement-root.md).

Observe que o recurso de revisões de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida adquirida ou de avaliação do Azure AD Premium P2 ou EMS e5.
Antes de criar um controle de revisão, programa ou programa do Access, um administrador deve ter sido previamente integrado para preparar os recursos do [programControlType](programcontroltype.md) e do [businessFlowTemplate](businessflowtemplate.md) . A organização pode se integrar às revisões do Azure AD Access ou, no caso de revisões de acesso das funções do Azure AD ou das funções de assinatura do Azure, o PIM do Azure AD.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão do Access.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do Access com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Criar um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualizar um accessReview. |
|[Listar accessReviews](../api/accessreview-list.md) |    coleção [accessReview](accessreview.md) |    Listar accessReviews para um businessFlowTemplate. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) |      coleção [UserIdentity](useridentity.md)| Obter os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicionar um revisor a um accessReview. |
|[Remover revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remover um revisor de um accessReview. |
|[Listar decisões accessReview](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como revisor, obtenha as minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Parar um accessReview. |
|[Redefinir decisões do accessReview](../api/accessreview-reset.md) |     Nenhum.   |   Redefina as decisões em um accessReview em andamento.|
|[Aplicar decisões accessReview](../api/accessreview-apply.md) |     Nenhum.   |   Aplique as decisões de um accessReview concluído.|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | coleção [businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriados para as revisões do Access.|
|[Criar programa](../api/program-create.md) |   [programa](program.md)   |   Criar um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  coleção [Program](program.md)|   Obtenha uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção de controles de um programa.|
|[Programa de atualização](../api/program-update.md) |   [programa](program.md)|  Atualizar um programa.|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicionar um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remover um programControl de um programa.|
|[Listar programControls](../api/programcontrol-list.md) | coleção [programControl](programcontrol.md)| Listar controles em todos os programas no locatário.|
|[Listar programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de permissão de aplicativo e função

As funções de diretório a seguir são necessárias para um usuário de chamada gerenciar revisões, programas e controles do Access.

| Recurso de destino | Operation | Permissões de aplicativos | Função de diretório necessária do usuário de chamada |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) de uma função do Azure AD | Leitura | AccessReview. Read. All ou AccessReview. ReadWrite. All | Administrador global, leitor global, administrador de segurança, leitor de segurança ou administrador de função privilegiada |
|[accessReview](accessreview.md) de uma função do Azure AD | Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador global ou administrador de função privilegiada |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Leitura | AccessReview. Read. All, AccessReview. ReadWrite. Membership ou AccessReview. ReadWrite. All | Administrador global, leitor global, administrador de segurança, leitor de segurança ou administrador de usuários |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Criar, atualizar ou excluir | AccessReview. ReadWrite. Membership ou AccessReview. ReadWrite. All | Administrador global ou administrador de usuário |
| [programas](program.md) e [programControl](programcontrol.md)| Leitura | ProgramControl. Read. All ou ProgramControl. ReadWrite. All |  Administrador global, leitor global, administrador de segurança, leitor de segurança ou administrador de usuários |
| [programas](program.md) e [programControl](programcontrol.md) | Criar, atualizar ou excluir | ProgramControl.ReadWrite.All | Administrador global ou administrador de usuário |

Além disso, um usuário que é um revisor atribuído de uma revisão do Access pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com as revisões do Azure AD Access](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com as revisões do Azure AD Access](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Como um administrador pode gerenciar programas e controles para revisões do Azure AD Access](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


