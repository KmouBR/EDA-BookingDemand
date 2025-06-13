# 📊 Hotel Booking Demand Analysis

Análise exploratória de dados baseada no dataset [Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand), com insights sobre reservas, sazonalidade, cancelamentos, comportamento dos hóspedes e canais de distribuição.

![GitHub last commit](https://img.shields.io/github/last-commit/KmouBR/EDA-BookingDemand)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Libraries-Pandas%2C%20Seaborn%2C%20Matplotlib-yellowgreen)

---

## 🧠 Objetivo

Investigar o comportamento das reservas em hotéis, identificar padrões de cancelamentos, sazonalidade da demanda e variáveis que influenciam na experiência do hóspede.

---

## 🔍 Perguntas que guiamos na análise:

1. Qual é a proporção de reservas canceladas?
2. Qual a distribuição entre tipos de hotel (City vs Resort)?
3. Qual é o perfil médio dos hóspedes?
4. Existe diferença no número de noites entre tipos de hotel?
5. Como o tipo de cliente se relaciona com cancelamentos?
6. A antecedência da reserva afeta o cancelamento?
7. Quais meses têm maior número de reservas? Existe sazonalidade?
8. Quais os países de origem mais frequentes?
9. Quais canais de distribuição geram mais reservas e cancelamentos?
10. Existem clientes fiéis que repetem reservas?

---

## 🔎 Respostas que guiamos da Análise

1. Em média 37% das reservas são canceladas, sugerindo que melhore as estratégias da reserva. É possível notar isso sabendo que pela column "is_canceled" ser do tipo booleana (valor 0 e 1) a média é tendenciosa a porcentagem do dado.
2. A Distribuição de reservas para o City Hotel está com a demanda de 66.4% já a do Resort com a metade desse valor em 33.5%.
3. Pela média, cada reserva possui 2 adultos sendo 0.1 crianças e 0.1 bebês. Isso indica que a maioria das reservas são de casais ou adultos viajando sozinhos, com pouca presença de crianças e ainda menos de bebês ( quase nulos ).
4. Sim, há diferença. O Resort Hotel apresenta em média 3.4 noites, enquanto o City Hotel tem média de 2.3 noites por reserva. Isso mostra que hóspedes costumam ficar mais tempo em resorts, possivelmente por se tratar de estadias de lazer, enquanto os hotéis de cidade atendem estadias mais curtas, talvez a trabalho. Acompanhado juntamente do p-value com evidência forte da hipótese ser verdadeira.
5. Os clientes "Transient" apresentam a maior taxa de cancelamento, com cerca de 41%, seguidos pelos "Transient-Party". Já clientes "Contract" praticamente não cancelam. Isso sugere que reservas corporativas ou com contrato fixo são mais confiáveis, enquanto clientes individuais são mais voláteis.
6. Quanto maior a antecedência da reserva, maior a chance de cancelamento. Reservas feitas com mais de 6 meses de antecedência possuem taxa de cancelamento acima de 50%, enquanto reservas de última hora (até 30 dias) têm taxa menor que 20%. Isso sugere que quanto mais cedo a reserva, maior a chance do plano mudar.
7. Sim existe sazonalidade clara e verídica. Os meses com maior número de reservas são Julho e Agosto, já os meses de janeiro e dezembro tem volume bem menor, mas isso é comum lembrando que o verão europeu ocorre nesse período de pico de reservas (Julho e Agosto).
8. Temos 41% do dataset ocupado por Portugal, 10% do Reino Unido e 8% da França, esses são os 3 países mais frequentes de Booking Demand. Nota-se através disso que o Hotel atende principalmente turistas da Europa.
9. O canal mais usado é o TA/TO (Agências de Viagem e Operadoras de Turismo), com mais de 80% das reservas. Porém, ele também apresenta alta taxa de cancelamento 42%. Já o canal “Direct” (reserva direta com o hotel) tem menos reservas, mas menor taxa de cancelamento 20%. Isso indica que reservas diretas são mais confiáveis.
10. Apenas 3% dos hóspedes são clientes repetentes, o que indica baixa fidelidade. A grande maioria das reservas vem de novos clientes. Isso pode indicar um foco maior em turistas ocasionais do que em fidelização de clientes.
    
---

## ⚙️ Tecnologias usadas

- Python 3.9+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 💡 Insights relevantes

- A taxa média de cancelamentos é de aproximadamente **37%**.
- Hotéis urbanos têm o dobro da demanda dos resorts.
- Reservas feitas com **muita antecedência** tendem a ter maior taxa de cancelamento.
- **Julho e Agosto** são os meses de pico, principalmente para resorts — indicando forte sazonalidade de verão.
- Portugal é o país com maior origem de hóspedes (~41% do total).

---

## 🧑‍💻 Autor

Feito com 💡 e curiosidade por Rafael Torres

---

## 📬 Feedback

Fique à vontade para abrir issues, sugerir melhorias ou apenas trocar uma ideia!
