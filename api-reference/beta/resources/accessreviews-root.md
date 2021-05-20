---
title: Avaliações de acesso do Azure AD - herdada
description: Você pode usar as análises de acesso do Azure AD para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário. Esta documentação atende às APIs herdas.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f8be8cb35add43d85b12bb3d466821ed8fd579a3
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579736"
---
# <a name="azure-ad-access-reviews-deprecated"></a>Avaliações de acesso do Azure AD (preteridas)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Você pode usar as análises de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.

Cenários de cliente típicos para análises de acesso de associações de grupo e acesso a aplicativos são:

- Os clientes podem revisar e certificar o acesso de usuários convidados usando análises de acesso de seu acesso a aplicativos e associações de grupos. Os revisadores podem usar as informações fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso de funcionários a aplicativos e associações de grupo com avaliações de acesso.

- Os clientes podem coletar controles de revisão de acesso em programas que são relevantes para sua organização acompanhar análises de conformidade ou aplicativos sensíveis a riscos.

Há também um recurso relacionado para que os clientes revisem e certifiquem as atribuições de função de usuários administrativos que são atribuídas a funções do Azure AD, como Administrador Global ou funções de assinatura do Azure.  Esse recurso está incluído no [Azure AD Privileged Identity Management](privilegedidentitymanagement-root.md).

Observe que o recurso de análises de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida comprada ou de avaliação do Azure AD Premium assinatura P2 ou EMS E5.
Antes de criar uma revisão de acesso, programa ou controle de programa, um administrador deve ter feito a integração anterior para preparar os recursos [programControlType](programcontroltype.md) e [businessFlowTemplate.](businessflowtemplate.md) A organização pode entrar em análises de acesso ao Azure AD ou, no caso de avaliações de acesso de funções do Azure AD ou funções de assinatura do Azure, PIM do Azure AD.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obter uma revisão de acesso com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Listar accessReviews](../api/accessreview-list.md) |    [Coleção accessReview](accessreview.md) |    Listar accessReviews para um businessFlowTemplate. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) |      [Coleção userIdentity](useridentity.md)| Obter os revisores de um accessReview. |
|[Adicionar o revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicione um revisor a um accessReview. |
|[Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remova um revisor de um accessReview. |
|[Listar decisões do accessReview](../api/accessreview-listdecisions.md) |      [Coleção accessReviewDecision](accessreviewdecision.md)| Obter as decisões de um accessReview.|
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) |     [Coleção accessReviewDecision](accessreviewdecision.md)| Como revisor, receba minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete aos revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Pare um accessReview. |
|[Redefinir as decisões do accessReview](../api/accessreview-reset.md) |     Nenhum.   |   Redefinir as decisões em um accessReview em andamento.|
|[Aplicar decisões do accessReview](../api/accessreview-apply.md) |     Nenhum.   |   Aplicar as decisões de um accessReview concluído.|
|[Listar businessFlowTemplates](../api/businessflowtemplate-list.md) | [Coleção businessFlowTemplate](businessflowtemplate.md)| Obter os modelos de fluxo de negócios apropriados para acessar avaliações.|
|[Criar programa](../api/program-create.md) |   [program](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Excluir um programa.|
|[Listar programas](../api/program-list.md) |  [conjunto de](program.md) programas|   Obter uma coleção de todos os programas.|
|[Listar programControls de um programa](../api/program-listcontrols.md) |      [Coleção programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Atualizar programa](../api/program-update.md) |   [program](program.md)|  Atualize um programa.|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remova um programControl de um programa.|
|[Listar programControls](../api/programcontrol-list.md) | [Coleção programControl](programcontrol.md)| Listar controles em todos os programas no locatário.|
|[Listar programControlTypes](../api/programcontroltype-list.md) | [Coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e permissão de aplicativo

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie avaliações, programas e controles de acesso.

| Recurso Target | Operation | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) de uma função do Azure AD | Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Função Privilegiada |
|[accessReview](accessreview.md) de uma função do Azure AD | Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Função Privilegiada |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Ler | AccessReview.Read.All, AccessReview.ReadWrite.Membership ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
|[accessReview](accessreview.md) de um grupo ou aplicativo | Criar, atualizar ou excluir | AccessReview.ReadWrite.Membership ou AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |
| [program](program.md) and [programControl](programcontrol.md)| Ler | ProgramControl.Read.All ou ProgramControl.ReadWrite.All |  Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| [program](program.md) and [programControl](programcontrol.md) | Criar, atualizar ou excluir | ProgramControl.ReadWrite.All | Administrador Global ou Administrador de Usuário |

Além disso, um usuário que é um revistor atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Como um administrador pode gerenciar programas e controles para avaliações de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


