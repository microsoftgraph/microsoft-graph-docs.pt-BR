---
title: Revisões de acesso do Azure AD (todos os recursos)
description: Você pode usar as revisões de acesso do Azure AD para configurar revisões de acesso única ou recorrentes para atestado dos direitos de acesso do usuário. Esta documentação atende às APIs herddas.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 0c616b20ac6c3dfc00ffdae319978a6bce60db5f
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292025"
---
# <a name="azure-ad-access-reviews-for-resources-excluding-groups"></a>Revisões de acesso do Azure AD (para recursos excluindo grupos)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Você pode usar as revisões de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar revisões de acesso única ou recorrentes para atestado dos direitos de acesso do usuário.

Cenários típicos de clientes para revisões de acesso de associações de grupo e acesso a aplicativos são:

- Os clientes podem revisar e certificar o acesso de usuários convidados usando revisões de acesso de seu acesso a aplicativos e associações de grupos. Os revisadores podem usar as ideias fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso de funcionários a aplicativos e associações de grupo com revisões de acesso.

- Os clientes podem coletar controles de revisão de acesso em programas relevantes para a sua organização para rastrear análises de aplicativos de conformidade ou de risco.

Há também um recurso relacionado para que os clientes revisem e certifiquem as atribuições de função de usuários administrativos que estão atribuídos a funções do Azure AD, como Administrador Global ou funções de assinatura do Azure.  Esse recurso está incluído no [Azure AD Privileged Identity Management](privilegedidentitymanagement-root.md).

Observe que o recurso de revisões de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário onde uma revisão de acesso está sendo criada deve ter uma assinatura válida adquirida ou de avaliação do Azure AD Premium P2 ou EMS E5.
Antes de criar uma revisão de acesso, programa ou controle de programa, um administrador deve ter sido previamente onboardado para preparar os recursos [programControlType](programcontroltype.md) e [businessFlowTemplate.](businessflowtemplate.md) A organização pode fazer a integração às revisões de acesso do Azure AD ou, no caso de revisões de acesso de funções do Azure AD ou funções de assinatura do Azure, PIM do Azure AD.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com os recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obter uma revisão de acesso com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Exclua um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Listar accessReviews](../api/accessreview-list.md) |    [coleção accessReview](accessreview.md) |    Listar accessReviews para um businessFlowTemplate. |
|[Listar revisores de accessReview](../api/accessreview-listreviewers.md) |      [coleção userIdentity](useridentity.md)| Obter os revisores de um accessReview. |
|[Adicionar o revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicione um revisor a um accessReview. |
|[Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remover um revisor de um accessReview. |
|[Listar decisões de accessReview](../api/accessreview-listdecisions.md) |      [coleção accessReviewDecision](accessreviewdecision.md)| Obter as decisões de um accessReview.|
|[Listar minhas decisões de accessReview](../api/accessreview-listmydecisions.md) |     [coleção accessReviewDecision](accessreviewdecision.md)| Como revisor, receba minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete aos revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Pare um accessReview. |
|[Redefinir decisões de accessReview](../api/accessreview-reset.md) |     Nenhum.   |   Redefinir as decisões em um accessReview em andamento.|
|[Aplicar decisões de accessReview](../api/accessreview-apply.md) |     Nenhum.   |   Aplicar as decisões de um accessReview concluído.|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | [Coleção businessFlowTemplate](businessflowtemplate.md)| Obter os modelos de fluxo de negócios apropriados para acessar revisões.|
|[Criar programa](../api/program-create.md) |   [programa](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  [coleção de](program.md) programas|   Obter uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      [coleção programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Atualizar programa](../api/program-update.md) |   [programa](program.md)|  Atualizar um programa.|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remover um programControl de um programa.|
|[Listar programControls](../api/programcontrol-list.md) | [coleção programControl](programcontrol.md)| Listar controles em todos os programas no locatário.|
|[Listar programControlTypes](../api/programcontroltype-list.md) | [Coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de permissão de aplicativo e função

As funções de diretório a seguir são necessárias para que um usuário chamado gerencie revisões de acesso, programas e controles.

| Recurso de destino | Operation | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) de uma função do Azure AD | Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Função Privilegiada |
|[accessReview](accessreview.md) de uma função do Azure AD | Criar, Atualizar ou Excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Função Privilegiada |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Ler | AccessReview.Read.All, AccessReview.ReadWrite.Membership ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Criar, Atualizar ou Excluir | AccessReview.ReadWrite.Membership ou AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |
| [program](program.md) and [programControl](programcontrol.md)| Ler | ProgramControl.Read.All ou ProgramControl.ReadWrite.All |  Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| [program](program.md) and [programControl](programcontrol.md) | Criar, Atualizar ou Excluir | ProgramControl.ReadWrite.All | Administrador Global ou Administrador do Usuário |

Além disso, um usuário que é um revisador atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com revisões de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com revisões de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Como um administrador pode gerenciar programas e controles para revisões de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


