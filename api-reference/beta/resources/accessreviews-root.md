---
title: Analisa de acesso do Azure AD
description: Você pode usar o Windows Azure AD acessar revisões para configurar o acesso de ocorrência única ou recorrente avaliações de certificação de direitos de acesso do usuário.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 212af4ad8519f7ec54fb56ceffee0a0d4de16027
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516410"
---
# <a name="azure-ad-access-reviews"></a>Analisa de acesso do Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o [acesso do Azure AD analisa](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar uma única vez ou recorrente access analisa para certificação dos direitos de acesso do usuário.

Cenários típicos de clientes para acesso analisa de associações de grupo e acesso ao aplicativo são:
   
- Os clientes podem examinar e certificar o acesso de usuário convidado usando revisões de acesso de seu acesso aos aplicativos e as associações de grupos. Os revisores podem usar as ideias fornecidos com eficiência decidir se convidados devem ter acesso contínuo.
      
- Os clientes podem examinar e certificar o acesso do funcionário aos aplicativos e associações com as revisões de acesso de grupo.
   
- Os clientes podem coletar acessar os controles de revisão em programas que são relevantes para a sua organização acompanhar as revisões para aplicativos de risco confidenciais ou de conformidade.

Também é um recurso relacionado para que os clientes revisem e certificar as atribuições da função de usuários administrativos que estão atribuídos às funções do Azure AD, como as funções de assinatura de Administrador Global ou do Windows Azure.  Esse recurso está incluído no [Windows Azure AD privilegiado gerenciamento de identidade](privilegedidentitymanagement-root.md).

Observe que o recurso de avaliações de acesso, incluindo a API, é incluído no Windows Azure AD Premium P2. 

## <a name="methods"></a>Métodos

Aqui está a lista dos métodos fornecidos pelo Windows Azure AD acessar as revisões.  

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do access com uma id específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Exclua um accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Listar accessReview revisores](../api/accessreview-listreviewers.md) |      coleção [userIdentity](useridentity.md)| Obtenha os revisores de um accessReview. |
|[Adicionar Revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicione um revisor a um accessReview. |
|[Remover accessReview revisor](../api/accessreview-removereviewer.md) | Nenhum.  |   Remova um revisor de um accessReview. |
|[Lista accessReview decisões](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar meus decisões accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como um revisor, obtenha Minhas decisões de um accessReview.|
|[Enviar accessReview lembrete](../api/accessreview-sendreminder.md) |        Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) |     Nenhum.   |   Pare uma accessReview. |
|[Redefinir accessReview decisões](../api/accessreview-reset.md) |     Nenhum.   |   Redefina as decisões em um accessReview em andamento.|
|[Aplicar accessReview decisões](../api/accessreview-apply.md) |     Nenhum.   |   Aplique as decisões de um accessReview concluída.|
|[Lista businessFlowTemplates](../api/businessflowtemplate-list.md) | coleção [businessFlowTemplate](businessflowtemplate.md)| Obtenha os modelos de fluxo de negócios apropriado para acessar as revisões.|
|[Criação de programa](../api/program-create.md) |   [programa](program.md)   |   Crie um novo programa.|
|[Excluir programa](../api/program-delete.md) |   Nenhum.   |   Exclua um programa.|
|[Lista de programas](../api/program-list.md) |  coleção de [programa](program.md)|   Obtenha uma coleção de todos os programas.|
|[Lista programControls de um programa](../api/program-listcontrols.md) |      coleção [programControl](programcontrol.md)| Obter uma coleção dos controles de um programa.|
|[Programa de atualização](../api/program-update.md) |   [programa](program.md)|  Atualize um programa.|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|
|[Excluir programControl](../api/programcontrol-delete.md) |     Nenhum.   |   Remova um programControl de um programa.|
|[Lista programControls](../api/programcontrol-list.md) | coleção [programControl](programcontrol.md)| Controles de lista com todos os programas no inquilino.|
|[Lista programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Lista os tipos de controle do programa. |


## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso de usuário com acesso do Azure AD analisa](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidado com acesso do Azure AD analisa](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Como um administrador pode gerenciar programas e avaliações de acessar controles para o Windows Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviews-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
