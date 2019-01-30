---
title: tipo de enum teamSpecialization
description: Descreve o caso de uso especial para uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640319"
---
# <a name="teamspecialization-enum-type"></a>tipo de enum teamSpecialization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica se a [equipe](../resources/team.md) destina-se de um caso de uso específico. Especialização cada [equipe](../resources/team.md) tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso. O padrão é 'Nenhum'.

## <a name="members"></a>Membros

| Membro             | Valor | Descrição                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | Tipo de uma equipe que dá a experiência de equipe padrão padrão.          |
| educationStandard  | 1     | Equipe criada por um usuário de educação. Todas as equipes criadas pelo usuário de educação são do tipo Edu. |
| educationClass     | 2     | Experiência otimizada para uma classe de equipe. Isso permite que a segmentação de recursos entre O365. |
| educationProfessionalLearningCommunity | 3 | Experiência otimizada para um PLC da equipe. Saiba mais sobre PLC [aqui](https://en.wikipedia.org/wiki/Professional_learning_community). |
| educationStaff     | 4     |  Tipo de equipe para uma experiência otimizada para as equipes em uma organização, onde um líder de equipe, como uma entidade de segurança, é o administrador e professores são membros de uma equipe que vem com um bloco de anotações especializado. Para obter mais detalhes, consulte o [Bloco de anotações do OneNote da equipe educacional](https://www.onenote.com/staffnotebookedu). |
| unknownFutureValue | 7     | Sentinel valor reservado como um espaço reservado para expansão futura do enum. |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
